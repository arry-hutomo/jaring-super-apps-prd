# Jaring Super Apps - Product Requirements Document (PRD)

**Nama Produk** : Jaring Super Apps (Jaring Hijau Nusantara)  
**Versi**       : 1.0  
**Tanggal**     : 31 Maret 2026  
**Platform**    : Progressive Web App (PWA) – Mobile Web App (Mobile-First)  
**Product Owner**: Amati Indonesia  


## Database Schema (Utama)

Berikut adalah struktur database utama:

```mermaid
erDiagram
    users {
        uuid id PK
        string phone
        string name
        string role "Petani/Mentor/Admin"
        string token
        string level "Basic/Intermediate/Advanced"
    }
    communities {
        uuid id PK
        uuid user_id FK
        string location
        string commodities
        decimal target_kg
        decimal dana_total
    }
    harvests {
        uuid id PK
        uuid community_id FK
        string commodity
        date harvest_date
        int weight_kg
        string quality "Grade A/B"
        string photo_url
    }
    damages {
        uuid id PK
        uuid community_id FK
        string description
        string priority "Low/Medium/High"
        date reported_date
        string status "Open/Closed"
    }
    reports {
        uuid id PK
        uuid community_id FK
        string type
        decimal amount
        string status "Approved/Revisions/Rejected"
    }

    users ||--o{ communities : "memiliki"
    communities ||--o{ harvests : "menghasilkan"
    communities ||--o{ damages : "melaporkan kerusakan"
    communities ||--o{ reports : "membuat laporan"
