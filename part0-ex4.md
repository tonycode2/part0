```mermaid
sequenceDiagram
participant browser
participant server


    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    Note left of server: POST sent with the information of the note ({note:string, date: Date()}). This also gets the new list of notes
    server-->>browser: [{ "content": "HTML is easy", "date": "2023-1-1" }, ... ]

    Note right of browser: This shows the already existing notes and the new note at the end.


```
