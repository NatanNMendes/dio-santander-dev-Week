# Santander Dev Week
Java RESTful API criada para a Santander Dev Week 2023
# Diagrama de Classes
```mermaid
classDiagram
    class User {
        +String name
    }

    class Account {
        +String number
        +String agency
        +float balance
        +float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +float limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *-- "N" Account : has
    User "1" *-- "N" Feature : has many
    User "1" *-- "N" Card : has
    User "1" *-- "N" News : has many
```
