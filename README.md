# Campus — mon espace étudiant

Un espace en français pour un étudiant en troisième année de marketing à HEC Rabat : tableau de bord, planning, suivi des devoirs, fiches personnelles, quiz avec explications, minuteur et repères pour la vie à Rabat.

## Lancer le site

Aucune dépendance ni compilation nécessaire. Depuis le dépôt :

```sh
python3 -m http.server 3000
```

Ouvrir le site servi sur le port 3000 dans un navigateur. Les fichiers peuvent aussi être hébergés sur un hébergement statique HTTPS.

## Données et limites

Les données sont enregistrées dans le stockage local du navigateur, sans compte ni synchronisation. L’espace « Ma vie à Rabat » permet d’exporter et de restaurer une sauvegarde JSON ; l’import remplace les données présentes. Ne pas conserver de documents personnels sensibles dans les fiches. Le minuteur nécessite une page ouverte et ne produit pas de notification système. Les objectifs se réinitialisent manuellement.

Les fiches et quiz sont des introductions générales au marketing, sans affiliation officielle avec HEC Rabat. Ils sont à compléter avec les cours et les consignes des enseignants. Aucun service d’IA, notification, calendrier externe ou service bancaire n’est connecté. Les conseils administratifs doivent être vérifiés auprès des organismes compétents.

Les polices Google Fonts sont facultatives : le site utilise des polices de remplacement si elles sont inaccessibles.

## Vérification

```sh
node --check app.js
```

Vérifier dans un navigateur : création et persistance d’une session, enregistrement d’une fiche, réponses aux quiz, pause et reprise du minuteur, calcul du budget, export/import et affichage mobile.
