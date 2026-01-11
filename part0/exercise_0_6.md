sequenceDiagram
    participant browser
    participant server

    Note right of browser: User types note and clicks "Save"
    Note right of browser: JS code adds new note to local list and rerenders
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    Note left of server: Server saves the note
    server-->>browser: 201 Created (JSON confirmation)
    deactivate server