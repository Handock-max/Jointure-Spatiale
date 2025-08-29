# Jointure Spatiale Google Colab

Ce repo contient un notebook Google Colab permettant de faire des **jointures spatiales** entre un fichier de points GPS et un GeoJSON de territoires.

## Utilisation

1. Ouvrir le notebook `googlecolab_notebook.ipynb` dans Google Colab : https://colab.research.google.com/
2. Installer les packages si nécessaire (le notebook inclut `!pip install geopandas folium openpyxl ipywidgets jedi`).
3. Uploader :
   - Votre fichier de points (CSV ou Excel avec colonnes latitude et longitude).
   - Votre fichier GeoJSON/Shapefile de territoires.
4. Choisir les paramètres CRS, tampon GPS et type de jointure.
5. Exécuter le notebook.
6. Télécharger le fichier ZIP généré contenant :
   - Le CSV des résultats de la jointure.
   - La carte interactive HTML.

## Exemples

- `ressources/togo_points.csv` : points fictifs au Togo.
- `ressources/togo_prefectures.geojson` : polygones réelles des préfectures du Togo pour test.

## Prérequis

Ce projet nécessite les bibliothèques suivantes :

- `geopandas`
- `folium`
- `pandas`
- `ipywidgets`
- `jedi`
- `openpyxl` (pour lire les fichiers Excel)

Vous pouvez installer ces dépendances avec pip :

```bash
pip install -r requirements.txt

