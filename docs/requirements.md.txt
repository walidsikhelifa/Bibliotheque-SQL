## Exigences Techniques

### Entités Principales
| Table     | Colonnes Clés               | Relations          |
|-----------|-----------------------------|--------------------|
| Books     | book_id, isbn               | 1-N avec Loans     |
| Members   | member_id, email            | 1-N avec Loans     |
| Loans     | loan_id, book_id, member_id | Clés étrangères    |

### Règles Métier
- Un livre ne peut être emprunté que s'il est disponible
- Durée maximale d'emprunt : 30 jours
- Un membre ne peut avoir plus de 5 emprunts simultanés

### Sécurité
- Validation des emails
- Chiffrement des données sensibles (non implémenté dans cette version)