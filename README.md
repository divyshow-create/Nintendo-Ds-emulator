# DS Pocket

Emulatore Nintendo DS che funziona offline, con tasti touch sullo schermo.
I giochi (.nds o .zip) li carichi tu dal telefono: restano sul dispositivo.

## Pubblicazione su GitHub Pages
1. Crea un repository (es. `ds-pocket`) e carica tutti i file di questa cartella nella radice.
2. Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)` → Save.
3. Dopo un paio di minuti l'app è su `https://<tuo-utente>.github.io/ds-pocket/`.

## Installazione sul telefono
- **iPhone (Safari):** apri il link → Condividi → *Aggiungi alla schermata Home*.
- **Android (Chrome):** apri il link → menu ⋮ → *Installa app* / *Aggiungi a schermata Home*.

Aprila una volta con internet: da lì in poi funziona anche offline.

## Aggiornare
Se cambi `index.html`, modifica `VERSION` in `sw.js` (es. `ds-pocket-v2`) così i telefoni scaricano la nuova versione.

Motore di emulazione: DeSmuME (WebAssembly).
