# Kreisker Kebab

Base statique du site vitrine `Kreisker Kebab`, reconstruite sur la meme ossature front-end que les precedents sites restaurant du dossier.

## Etat actuel

Le site couvre aujourd'hui :

- hero / accueil
- histoire et ambiance du restaurant
- menu complet par categories
- galerie photo avec placeholders documentes
- horaires, localisation et carte embarquee
- formulaire de reservation front-end
- mentions legales
- politique de confidentialite
- PWA minimale (`manifest.json`, favicons)
- bases SEO (`canonical`, Open Graph, Twitter, JSON-LD, `robots.txt`, `sitemap.xml`, `llms.txt`)

## Arborescence utile

- `index.html` : page principale
- `404.html` : page d'erreur
- `mentions-legales.html` : page legale
- `politique-confidentialite.html` : page de confidentialite
- `assets/css/styles.css` : styles globaux
- `assets/js/main.js` : interactions, menu mobile, reveals, accordions mobiles, reservation locale
- `assets/images/` : placeholders SVG et consignes de remplacement
- `assets/images/INDEX.md` : brief image par image
- `robots.txt` : directives crawl
- `sitemap.xml` : URLs publiees
- `manifest.json` : manifeste web app
- `llms.txt` : resume AI-friendly du site

## Lancer en local

Le site est statique. Une ouverture directe de `index.html` fonctionne pour la lecture simple, mais un serveur HTTP local est prefere pour tester la carte et les ancres proprement.

Exemple PowerShell :

```powershell
python -m http.server 4173
```

Puis ouvrir :

```text
http://127.0.0.1:4173
```

## Notes produit

- Les coordonnees publiques affichees reprennent les informations visibles sur Tripadvisor et Facebook au 24 mars 2026.
- Les visuels du dossier `assets/images/` sont des placeholders SVG remplacables, deja nommes selon leur usage dans la page.
- Le formulaire de reservation reste 100 % front-end : il prepare un recapitulatif local, copiable puis a confirmer par telephone ou Facebook.
