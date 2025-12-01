erDiagram
    CLASS {
        string Cno PK
        string Teacher
        int Csize
        string GradeNo
    }
    
    STUDENT {
        string Sno PK
        string Sname
        int Sage
        string Ssex
        string Cno FK
    }
    
    CLASS ||--o{ STUDENT : "1:n"
    STUDENT }o--|| CLASS : "belongs to"
