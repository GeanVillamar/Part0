```mermaid
sequenceDiagram
    participant browser
    participant server
    activate browser
    browser->>server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
    server-->>browser: State:302 Found
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    server-->>browser: State:200 OK
```



