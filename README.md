# devinedevine

Jeu de soirée « Sur le Front » : téléphone sur le front, les autres font deviner.
Incline vers le haut pour valider, vers le bas pour passer. Mode équipes, thèmes 18+, QR code de partage.

Jouer : https://funappi.github.io/devinedevine/

Made by funappi

## Ajouter ou mettre à jour des mots

Les mots peuvent être modifiés sans toucher au code : édite `words.json` (icône ✏️ sur GitHub, même depuis le téléphone), enregistre (« Commit changes »). Le jeu relit ce fichier à chaque ouverture, ou via Réglages > Mettre à jour les mots.

```json
{"themes":[
  {"id":"animaux","words":["Axolotl","Capybara"]},
  {"id":"noel","name":"Noël","em":"🎄","c":"#15803d","adult":false,"words":["Sapin","Guirlande"]},
  {"id":"metiers","replace":true,"words":["Pompier","Boulanger"]}
]}
```

- `id` d'un thème existant : les mots sont **ajoutés** (ajoute `"replace":true` pour remplacer la liste).
- nouvel `id` avec `name` : nouveau thème (`adult:true` pour le réserver au mode 18+).
- Identifiants existants : animaux, metiers, stars, films, series, dessins, chansons, marques, sports, bouffe, objets, monde, mimes, jeuxvideo, nostalgie, expressions, histoire, web, vacances, nord, contes, musique, coquin, aulit, accessoires, fantasmes, seduction, couple, galeres, mimesx, arrosee.
- Un thème retiré du fichier disparaît à la mise à jour suivante. Hors ligne, la dernière version connue est utilisée.
