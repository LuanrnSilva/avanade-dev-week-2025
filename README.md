# BootCamp Avanade
Java Restful API

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +Long Id
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +Long Id
        +String number
        +String agency
        +BigDecimal balance
        +BigDecimal limit
    }

    class Feature {
        +Long Id
        +String icon
        +String description
    }

    class Card {
        +Long Id
        +String number
        +BigDecimal limit
    }

    class News {
        +Long Id
        +String icon
        +String description
    }

    User "1" *-- "1" Account
    User "1" *-- "N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News
```
