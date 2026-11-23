# Site PokéTracker (GitHub Pages)

Page de présentation de l'app (anglais et français) et politique de confidentialité, sans dépendance ni étape de construction.

- `index.html` : page en anglais ;
- `fr/index.html` : version française ;
- `privacy.html` : politique de confidentialité (anglais, puis français à l'ancre `#fr`) ;
- `support.html` : assistance et questions fréquentes (anglais, puis français à l'ancre `#fr`), adresse « Support » de la fiche App Store ;
- `CNAME` : domaine personnalisé `getpoketracker.app` lu par GitHub Pages (23 novembre 2026) ;
- `images/icon.png` : icône de l'app (512 px, tirée de `Data/Assets.xcassets/AppIcon.appiconset/AppIcon.png`) ; la nouvelle icône à motif de Poké Ball et ses textes alternatifs sont en ligne depuis le 10 novembre 2026 (audit, point ASC-10, avec l'accord de l'utilisateur).

Le site ne montre aucune illustration de carte : elles appartiennent à leurs ayants droit. Des captures de l'app pourront être ajoutées à la publication (P8), après décision.

Contact : l'adresse `contact@getpoketracker.app` (depuis le 23 novembre 2026 ; redirection OVH vers la boîte Gmail du développeur, sans boîte propre, donc une réponse envoyée depuis Gmail montre l'adresse Gmail) et la page Issues du dépôt GitHub du site, sur `support.html` et `privacy.html` ; le lien « Contact » du pied des pages d'accueil ouvre un courriel vers cette adresse. Du 9 au 23 novembre 2026, l'adresse affichée était `everywherree@gmail.com` (audit avant App Store, point A10, à la demande de l'utilisateur). Jusqu'au 9 novembre, le contact se limitait aux tickets (décision du 4 novembre 2026), ce qui exposait à un refus au titre de la règle 1.5 d'Apple, surtout avec un abonnement payant.

## Adresses

Domaine `getpoketracker.app`, acheté chez OVH le 23 novembre 2026. L'app pointe vers ces adresses (`Utils/AppLinks.swift`, utilisées par Réglages › À propos et l'écran d'abonnement) :

- Site : https://getpoketracker.app/
- Politique de confidentialité : https://getpoketracker.app/privacy.html (pour App Store Connect)
- Assistance : https://getpoketracker.app/support.html (pour App Store Connect)

Les anciennes adresses `https://eeverywhereedv.github.io/poketracker-site/…`, encore dans les versions 1.0.5 et antérieures et sur la fiche publiée, redirigent vers le domaine : GitHub Pages le fait tant que le domaine personnalisé est réglé sur le dépôt. Ne pas retirer ce réglage ni renommer le dépôt.

**DNS** (zone OVH de `getpoketracker.app`) : quatre enregistrements A vers GitHub Pages (185.199.108.153 à 185.199.111.153), quatre AAAA (2606:50c0:8000::153 à 2606:50c0:8003::153), `www` en CNAME vers `eeverywhereedv.github.io.` ; MX et SPF d'OVH gardés pour la redirection du courriel. Le domaine `.app` impose HTTPS (liste HSTS des navigateurs) : le site ne s'ouvre qu'une fois le certificat émis par GitHub, puis « Enforce HTTPS » est coché.

**Publié** le 4 novembre 2026, avec l'accord de l'utilisateur, sur GitHub Pages depuis le dépôt public `eeverywhereedv/poketracker-site` (branche `main`, racine), comme le site de RiftTracker. Le dépôt contient une copie du dossier `site/` plus un fichier `.nojekyll` ; pour mettre le site à jour, recopier `site/` dans le dépôt et pousser (avec l'accord de l'utilisateur). Dernière publication le 23 novembre 2026 : bouton « Télécharger sur l'App Store » et bannière Safari (`apple-itunes-app`), l'app étant disponible dans l'Union européenne. Le 23 novembre 2026, ajout du fichier `CNAME` et passage au domaine `getpoketracker.app`. Si le nom public change (P7.1), le domaine, ces adresses et les liens de l'app changent avec lui.

## Vérifier en local

```bash
python3 -m http.server 8000 --directory site
```

Puis ouvrir http://localhost:8000/.
