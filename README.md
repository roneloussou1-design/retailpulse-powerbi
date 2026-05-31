# RetailPulse Analytics Platform - NordRetail

## Description
Plateforme analytique Power BI enterprise-grade pour NordRetail, 
enseigne de distribution paneuropéenne.

## Objectifs métier
- Suivre le chiffre d'affaires et les marges par région et catégorie
- Analyser la performance des magasins
- Monitorer les stocks et les ruptures
- Comprendre le comportement client (RFM, rétention, churn)

## Architecture Power BI
- 3 tables de faits : FactSales, FactInventory, FactCustomerEvents
- 5 dimensions : DimDate, DimProduct, DimCustomer, DimStore, DimPromotion
- Modèle en étoile avec relations one-to-many
- RLS dynamique par région

## Pages de rapport
- **Executive** : KPI globaux pour la direction
- **Catégorie** : Analyse produit pour les acheteurs
- **Magasins** : Performance des points de vente
- **Stocks** : Suivi des niveaux de stock
- **Client** : Segmentation et rétention

## Mesures DAX principales
- Total Revenue, Gross Margin %, Revenue YTD, Revenue YoY %
- Active Customers, Customer Retention Rate
- Stock Level, Days of Stock

## Sécurité RLS
- Rôle Regional Manager : accès filtré par région
- Rôle Executive : accès global

## DevOps
- Format PBIP versionné dans Git
- Branches : main, develop, feature/*
- Deployment Pipeline : DEV → TEST → PROD

## Limites du projet
- Source de données fictive (CSV)
- Certification non disponible sans licence Premium

## Améliorations futures
- Connexion à une vraie base de données
- Ajout de l'analyse prédictive
- Intégration avec Microsoft Fabric# retailpulse-powerbi
