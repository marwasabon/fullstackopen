
```mermaid
sequenceDiagram  
    participant User  
    participant Browser  
    participant Server  

    User->>Browser: Enters URL https://studies.cs.helsinki.fi/exampleapp/spa  
    Browser->>Server: Sends HTTP GET request for SPA resources  
    Server-->>Browser: Returns HTML, CSS, and JavaScript files  
    Browser->>Browser: Renders the SPA interface  
    Browser->>User: Displays initial view of notes app
