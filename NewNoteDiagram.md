```mermaid
 graph TD; 
 A-->B;
 B-->C;
 C-->D;
 D-->A;
```
sequenceDiagram
participant browser
participant server
activate browser
browser->>server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
browser-->server: State:302
desactive browser

