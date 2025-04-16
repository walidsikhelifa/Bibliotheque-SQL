##  Démarrage Rapide

### Installation
```bash
# Importation de la structure
mysql -u root -p < database/schema.sql

# Chargement des données de test
mysql -u root -p library_db < database/sample_data.sql