
![alt text](image-1.png)


![Chen Diagram](diagrama-chen1.drawio.png)


```mermaid

erDiagram
    STUDENT {
        long id_student PK
        string name_student
        string id_classroom FK
    }

    CLASSROOM {
        string id_classroom PK
        string classroom_description
    }

    COURSE {
        long id_course PK
        string course_name
        string id_classroom FK
    }

    STUDENT }o--|| CLASSROOM : "Study on"
    CLASSROOM ||--o{ COURSE : "Has"
    ```

