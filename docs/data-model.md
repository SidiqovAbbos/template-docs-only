# Data Model

<!-- This file will be populated by Copilot based on PLAN.md requirements -->

## Entity Relationship Diagram

```mermaid
erDiagram
    USER ||--o{ ORDER : places
    ORDER ||--|{ ORDER_ITEM : contains
    PRODUCT ||--o{ ORDER_ITEM : "ordered in"

    USER {
        uuid id PK
        string email
        string name
        timestamp created_at
    }

    ORDER {
        uuid id PK
        uuid user_id FK
        string status
        decimal total
        timestamp created_at
    }

    ORDER_ITEM {
        uuid id PK
        uuid order_id FK
        uuid product_id FK
        int quantity
        decimal price
    }

    PRODUCT {
        uuid id PK
        string name
        string description
        decimal price
        timestamp created_at
    }
```

## Entities
_Describe each entity, its fields, and relationships._

## Indexes
_List recommended database indexes._

## Migrations
_Describe the migration strategy._
