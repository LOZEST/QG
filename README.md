# QG Prépa

Un tableau de bord minimaliste pour la prépa TSI : tâches, objectifs, rappels, planning des khôlles et DS, notes, carnet d'erreurs et minuteur de travail.

Tout tient dans un seul fichier, `index.html` : pas de dépendance, pas de build.

## Mettre en ligne avec GitHub Pages

1. Crée un dépôt sur GitHub (par exemple `qg-prepa`).
2. Dépose `index.html`, `README.md` et `.nojekyll` à la racine du dépôt.
3. Dans le dépôt : **Settings → Pages → Build and deployment**, source **Deploy from a branch**, branche `main`, dossier `/ (root)`.
4. Après une minute, le site est en ligne à `https://<ton-pseudo>.github.io/qg-prepa/`.

En ligne de commande :

```bash
git init
git add index.html README.md .nojekyll
git commit -m "QG Prépa"
git branch -M main
git remote add origin https://github.com/<ton-pseudo>/qg-prepa.git
git push -u origin main
```

## Où sont mes données ?

Sur GitHub Pages, les données sont enregistrées dans le navigateur (localStorage), donc sur un seul appareil et un seul navigateur.
Pour les transférer : **Réglages → Copier mes données**, puis **Restaurer** sur l'autre appareil.

La version hébergée sur Claude (lien d'artefact) synchronise les données avec le compte Claude et peut s'installer comme app Mac. Les deux versions ne partagent pas leurs données.

## Contenu

- **Aujourd'hui** : tâches du jour, minuteur, khôlles/DS du jour et des 7 prochains jours, erreurs à revoir.
- **Planning** : khôlles du groupe 2, DS de TSI 1, concours blancs, créneaux SI du groupe A (année 2026-2027).
- **Notes** : moyennes pondérées par matière, import par copier-coller depuis École Directe.
- **Erreurs** : carnet d'erreurs avec révisions espacées (1, 3, 7, 21, 60 jours).
