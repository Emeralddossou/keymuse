# KeyMuse 🎹

Jouer un morceau entier sans connaître le solfège.

Importe un fichier MIDI, choisis ton instrument, puis utilise n'importe quelle touche de ton clavier. Chaque frappe joue la note — ou l'accord — qui vient ensuite.

**[Essayer KeyMuse](https://keymuse.onrender.com)**

## Deux façons de jouer

- **Guidé** — le morceau t'attend et t'indique quand appuyer.
- **Cadence** — le tempo continue quoi qu'il arrive. Si tu rates une note, elle est passée.

Le piano et la guitare sont disponibles directement dans le navigateur. Sur mobile, il suffit de toucher la zone centrale.

## Lancer le projet

Il n'y a rien à installer : ouvre simplement `index.html` dans ton navigateur.

Pour éviter les petites restrictions liées aux fichiers locaux, tu peux aussi lancer un serveur statique :

```bash
python3 -m http.server 8000
```

Puis ouvre `http://localhost:8000`.

## Morceaux de démo

Le dossier [`samples`](./samples) contient 20 morceaux MIDI libres de Debussy, Satie, Fauré et Purcell. Glisse-en un dans l'app pour commencer.

Les crédits et licences sont détaillés dans [`samples/README.md`](./samples/README.md).

## Comment ça marche ?

Tout tient dans un seul fichier HTML. Le navigateur analyse le MIDI, regroupe les notes simultanées en accords et fabrique les sons avec la Web Audio API. Aucun morceau n'est envoyé sur un serveur.

---

Fait pour le plaisir de jouer, même avec zéro cours de piano au compteur.
