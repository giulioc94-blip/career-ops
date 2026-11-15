# STATO

## 1) OBIETTIVO FINALE
Trovare ruoli per il candidato Giulio Curcio Terremoto (Dottore Commercialista, Revisore Legale, Cosenza) tra: Esperto di finanza agevolata (primario), Revisore legale senior (primario), Amministratore Delegato / CEO (secondario, evidenza di gestione da confermare).

## 2) ARCHITETTURA E REGOLE CHIAVE
- Layer utente (mai auto-aggiornato): `cv.md`, `config/profile.yml`, `modes/_profile.md`, `modes/_brief.md`, `portals.yml`.
- Nessuna fonte di fatti oltre al CV e alle dichiarazioni dirette del candidato.
- Mai inviare candidature senza revisione dell'utente.

## 3) COMPLETATO
- Dipendenze installate (`npm install`).
- `cv.md` creato dal PDF caricato.
- `config/profile.yml` e `portals.yml` generati con `onboard-write.mjs` (validati, 0 errori).
- `modes/_profile.md` riscritto con i tre archetipi.
- `modes/_brief.md` compilato per il triage.

## 4) IN CORSO / PROSSIMO PASSO ESATTO
- Compenso: il candidato indica target alto, non negoziabile verso il basso; cifra non fornita. `target_range` = descrizione qualitativa; nessun hard floor numerico.
- Evidenza di governo d'impresa dichiarata (2026-11-15): consulente esterno di numerose imprese, 2 incarichi di amministratore di fatto, 2 di revisore unico. Nomi, periodi e settori da completare in `cv.md`.
- Scan eseguito il 2026-11-15: 14873 annunci letti, 0 nuovi. Le 104 aziende in `portals.yml` sono tecniche (template): nessun titolo dei tre archetipi. Prossimo passo: sostituire le fonti con aziende/fonti italiane di finanza, revisione e amministrazione, poi rilanciare `node scan.mjs`.
- Vincolo geografico rimosso: il candidato lavora ovunque nel mondo (`portals.yml` location_filter vuoto; `_brief.md` aggiornato). Rescan: 2 nuove offerte, entrambe non pertinenti (Executive Assistant to the CEO; CEO Office strategy). Da non valutare.
- In attesa da candidato: dettagli degli incarichi (società, periodi, settori). Compenso: nessuna cifra indicativa, target alto e non negoziabile verso il basso.

## 5) FILE MODIFICATI E NOTE TECNICHE
- Nuovi file utente (gitignored): `cv.md`, `config/profile.yml`, `portals.yml`, `modes/_profile.md`, `modes/_brief.md`.
- `STATO.md` nella root (questo file).
- Lingua di output impostata a `it` in `config/profile.yml` (`language.output`).
