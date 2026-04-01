 * ## Client Role
 * - Initiates requests to the server
 * - Sends HTTP requests containing headers, methods, and payload data
 * - Receives and processes responses from the server
 * - Renders content (HTML, CSS, JavaScript) in a browser or application
 * - Manages user interactions and local state
 * - Handles network layer communication through HTTP/HTTPS protocols
 * 
 * ## Server Role
 * - Listens for incoming client requests on specific ports
 * - Processes requests based on HTTP methods (GET, POST, PUT, DELETE, etc.)
 * - Executes business logic and accesses databases or external services
 * - Generates and sends HTTP responses with appropriate status codes and data
 * - Manages server-side state, sessions, and authentication
 * - Serves static and dynamic content to clients
 * 
 * ## Web Communication Flow
 * 1. Client establishes TCP connection via network layers
 * 2. Client sends HTTP request to server
 * 3. Server receives and processes the request
 * 4. Server sends HTTP response back to client
 * 5. Client receives response and processes data
 * 6. Connection may be closed or reused (HTTP Keep-Alive)