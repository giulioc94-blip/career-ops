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
- Compenso target non definito: `config/profile.yml` → `compensation.target_range` = "da definire".
- Prossimo passo: chiedere al candidato il range retributivo e l'evidenza di gestione d'impresa per il ruolo CEO/AD; poi eseguire `node scan.mjs`.

## 5) FILE MODIFICATI E NOTE TECNICHE
- Nuovi file utente (gitignored): `cv.md`, `config/profile.yml`, `portals.yml`, `modes/_profile.md`, `modes/_brief.md`.
- `STATO.md` nella root (questo file).
- Lingua di output impostata a `it` in `config/profile.yml` (`language.output`).
