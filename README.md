# QG Prépa

Tableau de bord minimaliste pour la prépa TSI : tâches, objectifs, rappels, planning des khôlles et DS, notes, carnet d'erreurs et minuteur de concentration.

Tout tient dans `index.html` : pas de dépendance, pas de build.

## Mettre en ligne avec GitHub Pages

1. Copie `index.html`, `README.md` et `.nojekyll` à la racine du dépôt, puis **Commit** et **Push** dans GitHub Desktop.
2. Sur github.com, dans le dépôt : **Settings → Pages**, source **Deploy from a branch**, branche `main`, dossier `/ (root)`.
3. Une minute plus tard, le site est en ligne à `https://<ton-pseudo>.github.io/<nom-du-depot>/`.

## Où sont mes données ?

Sur GitHub Pages, les données restent dans le navigateur (un seul appareil, un seul navigateur).
Pour les transférer : **Réglages → Copier mes données**, puis **Restaurer** sur l'autre appareil.

## Minuteur de concentration

- Durées en un clic (25, 45, 60, 90 min) ou au choix, idem pour la pause.
- **Plein écran** : grand minuteur, −5 / +5 min, barre d'espace pour démarrer ou mettre en pause, Échap pour quitter.

## Planning

- Khôlles du groupe 2, DS de TSI 1, concours blancs, créneaux SI du groupe A (2026-2027).
- Survole une ligne puis **Modifier** pour changer la date, l'heure, le type, la matière ou le détail. **Ajouter un événement** en bas de la page.

## Relier à Calendrier (Apple)

1. Dans **Planning**, choisis le filtre (Tout, Khôlles ou DS), puis **Exporter vers Calendrier**.
2. Ouvre le fichier `prepa-planning.ics` téléchargé : Calendrier propose de l'importer. Choisis **Nouveau calendrier** → « Prépa ».
3. Alertes incluses : 30 min avant une khôlle, la veille à 18 h pour un DS sans heure.

Après de grosses modifications du planning, supprime le calendrier « Prépa » dans Calendrier et refais l'import pour éviter les doublons.

## Relier à Rappels (Apple)

Le site envoie tes tâches et rappels à un raccourci de l'app **Raccourcis**. À créer une seule fois :

1. Ouvre **Raccourcis** → **+** (nouveau raccourci), nomme-le exactement **`QG Rappels`**.
2. Ajoute l'action **Diviser le texte** : texte = *Entrée du raccourci*, séparateur = *Nouvelles lignes*.
3. Ajoute **Répéter avec chaque élément** sur le résultat (*Texte divisé*).
4. Dans la boucle, ajoute :
   - **Diviser le texte** : texte = *Élément de répétition*, séparateur = *Personnalisé* → `|`
   - **Obtenir l'élément de la liste** : *Premier élément* (c'est le titre)
   - **Obtenir l'élément de la liste** : *Dernier élément* de *Texte divisé* (c'est la date)
   - **Ajouter un nouveau rappel** : titre = premier élément, liste = « Prépa » (crée-la avant dans Rappels), **Alerte** = dernier élément.
5. Dans les réglages du raccourci (ⓘ), coche **Recevoir** → *Texte*.

Ensuite :
- **Tâches → Envoyer vers Rappels** envoie toutes les tâches à faire, avec une alerte à 8 h le jour prévu.
- **Rappels → Envoyer vers Rappels d'Apple** envoie les rappels à venir avec leur heure.

Le site envoie une ligne par élément, au format `titre|AAAA-MM-JJ HH:MM`.

## Notes et École Directe

**Notes → Importer depuis École Directe** : copie le tableau de notes sur École Directe, colle-le, vérifie l'aperçu, puis importe.

## Carnet d'erreurs

Chaque erreur revient à revoir après 1, 3, 7, 21 puis 60 jours tant que tu sais la refaire.
