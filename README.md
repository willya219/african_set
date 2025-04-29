# README - Africa Countries Dataset

## Description
Ce dataset contient des informations géographiques et administratives sur les pays africains. Il inclut des données telles que les codes ISO, les noms des pays, les régions, ainsi que des mesures géométriques liées à leur superficie et à leur périmètre.

## Colonnes

1. **FID** (Feature ID)  
   - Identifiant unique pour chaque enregistrement.  
   - Type : Entier  

2. **OBJECTID**  
   - Identifiant supplémentaire pour chaque pays.  
   - Type : Entier  

3. **ISO**  
   - Code ISO à trois lettres pour chaque pays.  
   - Type : Texte  
   - Exemple : `AGO` pour l'Angola, `EGY` pour l'Égypte.  

4. **NAME_0**  
   - Nom complet du pays.  
   - Type : Texte  
   - Exemple : `Angola`, `Egypt`.  

5. **Continent**  
   - Continent auquel appartient le pays (tous les pays de ce dataset sont en Afrique).  
   - Type : Texte  
   - Valeur : `Africa` pour tous les enregistrements.  

6. **Region**  
   - Sous-région africaine à laquelle le pays appartient.  
   - Type : Texte  
   - Valeurs possibles :  
     - `Eastern_Africa` (Afrique de l'Est)  
     - `Southern Africa` (Afrique australe)  
     - Vide (non spécifié pour certains pays)  

7. **Shape__Area**  
   - Superficie du pays en unités carrées (probablement en mètres carrés, mais l'unité exacte n'est pas précisée).  
   - Type : Nombre réel  
   - Exemple : `1319275625736.23` pour l'Angola.  

8. **Shape__Length**  
   - Périmètre ou longueur totale des frontières du pays en unités linéaires (probablement en mètres, mais l'unité exacte n'est pas précisée).  
   - Type : Nombre réel  
   - Exemple : `8268691.48474777` pour l'Angola.  

## Notes

- Certains champs **Region** sont vides, ce qui signifie que la sous-région n'est pas spécifiée pour ces pays.  
- Les données géométriques (`Shape__Area` et `Shape__Length`) sont très précises et peuvent être utilisées pour des analyses spatiales.  
- Les codes ISO sont conformes à la norme ISO 3166-1 alpha-3.  

## Exemple de données

| FID | OBJECTID | ISO | NAME_0                     | Continent | Region         | Shape__Area       | Shape__Length   |
|-----|----------|-----|----------------------------|-----------|----------------|-------------------|-----------------|
| 1   | 1        | AGO | Angola                     | Africa    |                | 1319275625736.23  | 8268691.48474777|
| 3   | 3        | BDI | Burundi                    | Africa    | Eastern_Africa | 27238231222.074   | 1133304.9827498 |
| 32  | 32       | MOZ | Mozambique                 | Africa    | Southern Africa| 872029959032.623  | 14175776.8743578|

## Utilisation potentielle

- Analyse géographique des pays africains.  
- Comparaison des superficies et des périmètres.  
- Cartographie et visualisation des données régionales.  

Pour toute question ou clarification supplémentaire, veuillez consulter la source originale des données ou les métadonnées associées.
