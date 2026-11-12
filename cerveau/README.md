# Cerveau Universel

Ton second cerveau en 3D. Chaque fichier est une planète-neurone, chaque dossier est une étoile, et ta racine est le noyau galactique. Des filaments forment la colonne et les vaisseaux, comme un vrai réseau neuronal à l'échelle de l'univers.

## Installer
1. Copie `index.html` dans `Documents\SecondBrain\_Cerveau3D\` (renomme-le `Cerveau 3D.html` si tu veux garder ton raccourci).
2. Ouvre-le avec **Chrome ou Edge**. Il faut Internet pour charger le moteur 3D.
3. Clique sur **Connecter mon SecondBrain** et choisis le dossier `SecondBrain`. L'analyse se fait entièrement sur ton PC.

## Utiliser
- **Recherche** (`Ctrl K` ou `/`) : fichiers, dossiers, contenu des fichiers texte, actions et souvenirs.
  - `>` au début : seulement les actions.
  - `#` au début : seulement les régions.
  - `Entrée` : y aller. `Maj+Entrée` : ouvrir ou lancer.
- **Actions** : ce sont les planètes à anneaux sur la moelle épinière. Ajoute les tiennes avec « + Action » (lien, fichier ou mémo).
- **Moteur de réorganisation** : il redistribue tout le cerveau.
  - **Anatomie** : selon tes dossiers.
  - **Thèmes** : selon le sens du contenu (TF-IDF + k-means, calculé en local).
  - **Types** : selon la nature du fichier.
  - **Chronologie** : du plus récent au plus ancien.
- **Plan de rangement** : transforme l'organisation affichée en vrais dossiers.
  1. Renomme les dossiers proposés.
  2. Télécharge `rangement.ps1` et `annulation.ps1`, et place-les à la racine de `SecondBrain`.
  3. Lance une simulation :
     `powershell -ExecutionPolicy Bypass -File .\rangement.ps1 -Simulation`
  4. Relance sans `-Simulation`.

  Les fichiers sont seulement déplacés, jamais supprimés. Le dossier `_Cerveau3D` n'est jamais touché.
- **⇩ Index** : exporte l'index en JSON pour le réimporter ailleurs.
