# Kit d'urgence cyber — PME suisses

Site statique Hugo en français pour aider les PME suisses romandes à réagir à un incident cyber.
Il rassemble des fiches d'action, les contacts utiles et un modèle minimal de registre des traitements LPD.
Le contenu est gratuit et réutilisable sous licence CC BY-SA 4.0.

## Contribuer

Forkez le dépôt, proposez vos changements dans une branche, puis ouvrez une pull request. Pour les coordonnées d'urgence ou les obligations légales, indiquez vos sources et la date de vérification.

## Tester et déployer localement

Installez [Hugo](https://gohugo.io/installation/), puis lancez le serveur de développement à la racine du dépôt :

```sh
hugo server
```

Le site sera disponible à l'adresse affichée par Hugo, généralement `http://localhost:1313/`. Pour générer les fichiers statiques de production :

```sh
hugo --minify
```

Chaque push sur `main` déclenche le workflow GitHub Actions et publie le dossier `public/` sur la branche `gh-pages`. Dans les paramètres GitHub Pages du dépôt, sélectionnez cette branche comme source de publication. Le fichier `static/CNAME` configure le domaine `urgence.guidecyber.ch`; configurez le DNS `urgence` comme CNAME vers le domaine GitHub Pages de votre compte.

## Licence

Le contenu est publié sous licence [Creative Commons Attribution – Partage dans les mêmes conditions 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/deed.fr).

**Avertissement : ce kit ne remplace pas un accompagnement professionnel.** Les obligations dépendent de votre situation, de votre secteur et de vos contrats. Vérifiez les consignes des autorités et de votre assurance.
