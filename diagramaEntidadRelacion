```mermaid
erDiagram
    USERS {
        uuid id PK
        string email
        string password_hash
        timestamp created_at
    }

    WALLET_BALANCES {
        uuid id PK
        uuid user_id FK
        string currency
        numeric amount
    }

    TRANSACTIONS {
        uuid id PK
        uuid user_id FK
        string type
        string from_currency
        string to_currency
        numeric from_amount
        numeric to_amount
        numeric rate_used
        timestamp rate_timestamp
        string status
        timestamp created_at
    }

    EXCHANGE_RATE_CACHE {
        uuid id PK
        string base_currency
        string target_currency
        numeric rate
        timestamp fetched_at
    }

    USERS ||--o{ WALLET_BALANCES : "posee"
    USERS ||--o{ TRANSACTIONS : "ejecuta"