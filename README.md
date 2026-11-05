# Il lusso ha due lingue

Sito editoriale su due campagne di lusso: **Rolls-Royce Ghost, teaser film (2020)** e
**Golden Goose, Born to Be a Super-Star (2025)**, analizzate con retorica, semiotica e il quadrato di Floch.

Testi e dati vengono da `ricerca.md` (fonte principale, non modificata). Le differenze sono in [VERIFICHE.md](VERIFICHE.md).

## Struttura

```
index.html  style.css  script.js  .nojekyll
assets/
  img/campagne/rolls-royce/   fotogrammi del teaser e illustrazione Post Opulence
  img/campagne/golden-goose/  foto della campagna e del racconto del marchio
  img/ai/                     illustrazioni teoriche generate con AI (SVG)
  img/grafiche/               favicon e texture
  fonts/                      Cormorant Garamond, Inter, Anton (licenza SIL OFL)
```

## Avvio in locale

```bash
python -m http.server 4173
```

Poi apri http://localhost:4173

## Comandi durante l'esposizione

| Comando | Effetto |
| --- | --- |
| Tasto **P** o pulsante **Presenta** | Avvia o chiude la presentazione a schermo intero (28 slide) |
| Frecce, barra spaziatrice, PagSu/PagGiù | Slide successiva o precedente |
| Home / Fine | Prima o ultima slide |
| Esc | Esce e torna alla slide raggiunta |
| Clic su un'immagine | Ingrandisce; clic di nuovo per lo zoom; frecce per scorrere |
| Trascina la linea argento in home (o frecce con il focus) | Sposta il confine: il titolo cambia carattere |
| Clic sulle schede del quadrato di Floch | Evidenzia l'angolo corrispondente |

## Pubblicare su GitHub Pages

Il sito è statico e usa solo percorsi relativi: non serve alcuna compilazione.

1. Crea un repository su GitHub e carica il contenuto di questa cartella.
2. Vai su **Settings → Pages**.
3. In **Source** scegli **Deploy from a branch**, poi `main` e `/ (root)`.
4. Dopo qualche minuto il sito è online su `https://TUO-UTENTE.github.io/NOME-REPO/`.

**Attenzione:** con GitHub Pages le immagini delle campagne diventano pubbliche. Sono opere protette
(© Rolls-Royce, Imagination, Cath Elliott, Golden Goose). I crediti e lo scopo didattico aiutano, ma non
sono una licenza: chiedi conferma al docente. Nota che su GitHub gratuito le Pages richiedono un repository
pubblico. Anche `ricerca.md` verrebbe pubblicato: toglilo dal repository se non vuoi.

## Immagini: cosa aggiungere o sostituire

Il sito è completo così com'è. Queste aggiunte sono facoltative.

| Dove | File | Cosa serve |
| --- | --- | --- |
| Golden Goose, «Nati per essere» | `assets/img/campagne/golden-goose/` | Scatti con le sneakers in primo piano. Sono su [The Impression](https://theimpression.com/golden-goose-super-star-ad-campaign-review), che blocca il download automatico: salvali a mano |
| Golden Goose, «Lo spot» | `index.html`, link `film-gg` | Se trovi il film sul canale YouTube ufficiale, aggiungi al link `data-embed="https://www.youtube-nocookie.com/embed/ID?autoplay=1"` per riprodurlo dentro il sito |
| Teoria, tutte le illustrazioni | `assets/img/ai/*.svg` | Oggi sono disegni vettoriali scritti da un'AI. Per versioni più pittoriche usa i prompt qui sotto e aggiorna i percorsi in `index.html` |

### Prompt per le illustrazioni

Stile comune: *editorial flat illustration, warm cream and black palette with champagne and antique gold accents, no text, no logos, no real brand.*

- **retorica**: a mouth speaking a word that turns into a golden fishing hook
- **semiotica**: a magnifying glass over a gold star, among abstract signs
- **segno-stella**: split image, a gold star on the left, a podium with a laurel wreath on the right
- **rosa**: split image, a red rose on the left, a red heart on the right
- **metafora**: a generic car silhouette wrapped in flowing silk, dark background
- **similitudine**: a human profile exhaling a thin breath of air
- **iperbole**: a gigantic perfume bottle in a street, tiny cars stopped in front of it
- **personificazione**: a worn generic sneaker with a speech bubble
- **antitesi**: one sphere split in half, polished on one side, cracked on the other
- **ironia**: an empty director's chair under a spotlight, dotted outline of missing shoes
- **sinestesia**: a sound wave turning into a fold of red velvet

## Crediti

- Fotogrammi del teaser Ghost: © Rolls-Royce Motor Cars / Imagination / Cath Elliott
- Illustrazione Post Opulence: © Rolls-Royce Motor Cars (PressClub, uso editoriale)
- Foto della campagna: © Golden Goose, foto Maik Schuster
- Timbri e attrezzi: © Golden Goose (racconto del marchio, non campagna)
- Video: incorporato da Vimeo (Cath Elliott); link a Instagram per Golden Goose
- Progetto scolastico a scopo didattico, non affiliato ai marchi citati
