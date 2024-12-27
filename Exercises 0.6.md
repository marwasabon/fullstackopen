```mermaid  
sequenceDiagram  
    participant User  
    participant Browser  
    participant Server  

    User->>Browser: Enters text into the note text field  
    Browser->>User: Displays entered text  

    User->>Browser: Clicks "Save" button  
    Browser->>Server: Sends POST request with note data  
    Note right of Server: (The data includes the note text)  

    Server->>Server: Processes the request (validate and store note)  
    Server-->>Browser: Responds with success message or new note data  

    Browser->>User: Displays confirmation message or updated notes list
