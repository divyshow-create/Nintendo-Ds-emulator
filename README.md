# DS Touch — Nintendo DS web emulator interface

Interfaccia mobile-first con pulsanti virtuali sullo schermo: D-pad, A/B/X/Y, L/R, Start e Select, selezione file `.nds` e pulsante fullscreen.

## Stato importante
Questa cartella contiene la UI e il caricamento di EmulatorJS tramite CDN. **Non è un pacchetto completamente offline**: il motore emulatore viene scaricato da Internet. Il browser legge la ROM localmente tramite un URL temporaneo, non la invia a un backend applicativo.

Per eseguire offline, scarica e ospita localmente i file del motore EmulatorJS (inclusi `loader.js`, i file JavaScript e WebAssembly del core melonDS e gli asset richiesti), poi modifica `EJS_pathtodata` in `index.html` al percorso locale, ad esempio `./data/`. Verifica le condizioni di licenza del motore e di tutti gli asset distribuiti.

## GitHub Pages
1. Carica `index.html` e `README.md` nella root di un repository.
2. Vai in **Settings → Pages**.
3. Seleziona **Deploy from a branch**, branch `main`, cartella `/(root)`.
4. Apri l'URL pubblicato e scegli una ROM `.nds` legalmente ottenuta.

## Note
- I giochi commerciali e i file BIOS non sono inclusi.
- L'emulazione dipende dal browser, dal dispositivo e dal supporto del core.
- I pulsanti virtuali inviano eventi tastiera; la compatibilità può variare in base alla versione del motore.
- Per un vero pacchetto offline, il motore WASM deve essere presente nel repository e non caricato da CDN.
