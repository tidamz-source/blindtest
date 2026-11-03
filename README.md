# Blindtest Live

Blindtest à buzzer : la musique passe sur le grand écran, les joueurs buzzent depuis leur téléphone et donnent leur réponse au micro.

## Mise en ligne (GitHub Pages)

1. Dépose `index.html` à la racine du dépôt.
2. *Settings > Pages* : *Deploy from a branch*, branche `main`, dossier `/ (root)`.
3. Le site est servi à `https://<pseudo>.github.io/<dépôt>/`. Ouvre-le toujours avec le `/` final, sans `index.html`.

## Spotify (optionnel, compte Premium)

1. Crée une app sur https://developer.spotify.com/dashboard en cochant **Web API** et **Web Playback SDK**.
2. Ajoute comme Redirect URI l'URL exacte du site (avec le `/` final). La page l'affiche dans le bloc Spotify.
3. Colle le Client ID dans la page, connecte-toi, puis importe une de tes playlists.

Seules tes propres playlists ou les playlists collaboratives sont lisibles. Le lecteur Spotify fonctionne sur ordinateur (Chrome, Edge, Firefox).

## Jouer

1. Sur le PC relié au vidéoprojecteur : ajoute tes MP3 (nom conseillé « Artiste - Titre.mp3 ») ou importe une playlist Spotify, règle les options, puis *Ouvrir la salle*.
2. Les joueurs scannent le QR code, entrent leur prénom et testent leur micro.
3. *Lancer la partie*. Au premier buzz, la musique s'arrête. Une réponse fausse relance la musique et le joueur est bloqué jusqu'à l'extrait suivant.

Variantes de réponse : sépare-les par « / » avec des espaces (ex. `Papaoutai / Papa où t'es`).

## À savoir

- Connexion peer-to-peer via le serveur public PeerJS, sans backend. Le Wi-Fi du lieu est plus fiable que la 4G.
- Si l'onglet de l'écran est rechargé, la partie et les scores sont perdus.
- iPhone : la dictée doit être activée (*Réglages > Général > Clavier > Dictée*).
