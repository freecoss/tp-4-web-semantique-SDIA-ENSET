# TP Web Sémantique - RDFa et SEO

## Description du Projet

Ce projet est un compte rendu de travaux pratiques sur le **Web Sémantique** et l'utilisation de **RDFa** pour améliorer le référencement (SEO) des pages web.

## Objectif

L'objectif de ce TP est de démontrer l'impact des annotations sémantiques RDFa sur le référencement et l'affichage des Rich Snippets dans les moteurs de recherche comme Google.

## Contenu du Projet

### Fichiers HTML

1. **recette_rdfa_seo.html**
   - Page web annotée avec RDFa et Schema.org
   - Contient des métadonnées structurées pour une recette de cuisine (Tajine de Poulet)
   - Optimisée pour les Rich Snippets Google
   - Annotations incluent : Recipe, AggregateRating, NutritionInformation, Review, HowToStep

2. **recette_sans_rdfa.html**
   - Version identique de la page mais SANS annotations RDFa
   - Permet de comparer l'impact du balisage sémantique
   - Même contenu visuel mais sans métadonnées structurées

### Comparaison

| Aspect | Avec RDFa | Sans RDFa |
|--------|-----------|-----------|
| Annotations sémantiques | ✅ Oui | ❌ Non |
| Rich Snippets Google | ✅ Supporté | ❌ Non supporté |
| Vocabulaire Schema.org | ✅ Implémenté | ❌ Absent |
| SEO optimisé | ✅ Oui | ⚠️ Basique |

## Technologies Utilisées

- **HTML5**
- **RDFa (Resource Description Framework in Attributes)**
- **Schema.org** - Vocabulaire pour les recettes
- **CSS3** - Design responsive et moderne

## Annotations RDFa Implémentées

- `vocab="https://schema.org/"` - Déclaration du vocabulaire
- `typeof="Recipe"` - Type de contenu (recette)
- `property="name"`, `property="description"` - Propriétés de base
- `property="recipeIngredient"` - Liste des ingrédients
- `property="recipeInstructions"` avec `typeof="HowToStep"` - Étapes de préparation
- `property="nutrition"` avec `typeof="NutritionInformation"` - Valeurs nutritionnelles
- `property="aggregateRating"` - Note moyenne
- `property="review"` - Avis clients

## Tests et Validation

Les pages peuvent être testées avec :
- [Google Rich Results Test](https://search.google.com/test/rich-results)
- [RDFa Play](https://rdfa.info/play/)

## Résultats

La version avec RDFa permet aux moteurs de recherche de :
- Afficher des Rich Snippets avec note, temps de préparation, calories
- Améliorer la visibilité dans les résultats de recherche
- Structurer les données pour une meilleure compréhension du contenu

## Auteur

École Normale Supérieure de Mohammedia

## Date

Avril 2025
