# Architecture - NordRetail Power BI

## Contexte
Plateforme analytique pour NordRetail, enseigne paneuropéenne.

## Modèle en étoile
- Choix du modèle en étoile pour performances et lisibilité DAX
- 3 tables de faits, 5 dimensions

## Import vs DirectQuery
- Choix Import pour performances optimales
- Données fictives CSV rechargées manuellement

## Sécurité
- RLS dynamique via USERPRINCIPALNAME()
- Table DimUser comme référentiel des accès

## Gouvernance
- Naming conventions appliquées
- Data dictionary documenté
- Best Practice Analyzer : 0 violations

## Déploiement
- Format PBIP versionné dans Git
- Pipeline DEV → TEST → PROD configuré
