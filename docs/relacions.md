# Relacions

## Relacions entre entitats

Les relacions indiquen com interactuen les entitats.

## Tipus de cardinalitat

### 1:1

Una entitat es relaciona amb una única altra entitat.

### 1:N

Una entitat es relaciona amb múltiples entitats.

### N:M

Múltiples entitats es relacionen entre si.

## Diagrama Mermaid

```mermaid
erDiagram
    ESTUDIANT ||--o{ INSCRIPCIO : realitza
    CURS ||--o{ INSCRIPCIO : conte
    PROFESSOR ||--o{ CURS : imparteix

    ESTUDIANT {
        int id_estudiant
        string nom
        string email
    }

    CURS {
        int id_curs
        string nom
        date inici
    }

    PROFESSOR {
        int id_professor
        string nom
        string especialitat
    }
```