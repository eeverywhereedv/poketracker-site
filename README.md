# Site PokéTracker (GitHub Pages)

Page de présentation de l'app (anglais et français) et politique de confidentialité, sans dépendance ni étape de construction.

- `index.html` : page en anglais ;
- `fr/index.html` : version française ;
- `privacy.html` : politique de confidentialité (anglais, puis français à l'ancre `#fr`) ;
- `support.html` : assistance et questions fréquentes (anglais, puis français à l'ancre `#fr`), adresse « Support » de la fiche App Store ;
- `images/icon.png` : icône de l'app (512 px, tirée de `Data/Assets.xcassets/AppIcon.appiconset/AppIcon.png`).

Le site ne montre aucune illustration de carte : elles appartiennent à leurs ayants droit. Des captures de l'app pourront être ajoutées à la publication (P8), après décision.

Contact : la page Issues du dépôt GitHub du site, sans adresse e-mail (décision de l'utilisateur le 4 novembre 2026). Apple demande un moyen simple de contacter le développeur (règle 1.5) : en cas de refus pour ce motif, ajouter une adresse e-mail à `support.html`.

## Adresses prévues

L'app pointe déjà vers ces adresses (`Utils/AppLinks.swift`, utilisées par Réglages › À propos et l'écran d'abonnement) :

- Site : https://eeverywhereedv.github.io/poketracker-site/
- Politique de confidentialité : https://eeverywhereedv.github.io/poketracker-site/privacy.html (pour App Store Connect)
- Assistance : https://eeverywhereedv.github.io/poketracker-site/support.html (pour App Store Connect)

**Publié** le 4 novembre 2026, avec l'accord de l'utilisateur, sur GitHub Pages depuis le dépôt public `eeverywhereedv/poketracker-site` (branche `main`, racine), comme le site de RiftTracker. Le dépôt contient une copie du dossier `site/` plus un fichier `.nojekyll` ; pour mettre le site à jour, recopier `site/` dans le dépôt et pousser (avec l'accord de l'utilisateur). Si le nom public change (P7.1), le dépôt, ces adresses et les liens de l'app changent avec lui.

## Vérifier en local

```bash
python3 -m http.server 8000 --directory site
```

Puis ouvrir http://localhost:8000/.
