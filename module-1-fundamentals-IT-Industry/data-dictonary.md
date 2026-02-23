
# E-Commerce App Data Dictionary

## Tables Overview

| Table Name | Purpose |
|-----------|---------|
| Users | Store customer and admin information |
| Products | Maintain product catalog |
| Categories | Product categories |
| Orders | Customer orders |
| OrderItems | Individual items in orders |
| Cart | Shopping cart items |
| Payments | Payment transaction records |
| Reviews | Product reviews and ratings |
| Inventory | Stock management |
| Addresses | Customer delivery addresses |

## Table Relationships

```
Users (1) ──→ (M) Orders
Users (1) ──→ (M) Reviews
Users (1) ──→ (M) Addresses
Users (1) ──→ (M) Cart

Products (1) ──→ (M) OrderItems
Products (1) ──→ (M) Reviews
Products (1) ──→ (M) Cart
Products (1) ──→ (M) Inventory

Categories (1) ──→ (M) Products

Orders (1) ──→ (M) OrderItems
Orders (1) ──→ (1) Payments
Orders (1) ──→ (1) Addresses

Inventory (1) ──→ (1) Products
```

## Key Fields by Table

- **Users**: UserID (PK), Email, Name, Password

- **Products**: ProductID (PK), CategoryID (FK), Name, Price, Description

- **Orders**: OrderID (PK), UserID (FK), OrderDate, Status

- **OrderItems**: OrderItemID (PK), OrderID (FK), ProductID (FK), Quantity, Price

- **Payments**: PaymentID (PK), OrderID (FK), Amount, Status, Method