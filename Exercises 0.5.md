flowchart TD  
    A[User] -->|Navigates to| B[Single Page App]  
    B -->|Renders Initial View| C[Input Area for New Note]  
    C -->|Enters Note Text| D[Save Button]  
    D -->|Clicks Save| E[AJAX POST Request to Server]  
    E -->|Server Saves Note| F[Server Response with New Note Data]  
    F -->|Update UI| G[Display New Note in Notes List]  
    G -->|Show Confirmation Message| H[User Sees New Note Added]
