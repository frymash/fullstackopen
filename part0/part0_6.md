```mermaid
    sequenceDiagram
    participant browser
    participant server


    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: JSON: {"message":"note created"}
    deactivate server

    Note right of browser: The browser stays on the same page and sends no further HTTP requests.
```