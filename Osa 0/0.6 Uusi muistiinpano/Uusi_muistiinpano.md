sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa JSON
    activate server
    server-->>browser: Status 201 Created - new note created
    deactivate server 
