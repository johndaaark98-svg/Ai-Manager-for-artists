# John Dark — Command Center

Centro di comando per il lancio del singolo **"Sembra mi piaccia"** — drop **17 luglio 2026, ore 12:00**.

App web a pagina singola, senza build e senza dipendenze: tutto dentro `index.html`.

## Cosa fa

- **Countdown** live al drop
- **Calendario** giugno/luglio cliccabile: tocchi un giorno e vedi cosa pubblicare, i task e le storie
- **Come girarlo** per ogni contenuto, tarato sui tuoi strumenti (iPhone 13 Pro Max / Nikon / GoPro)
- **Piano storie** giornaliero, con lo sticker giusto e il perché
- **Reference** (Pinterest / TikTok) per ogni contenuto e ogni storia
- **Log metriche** (views, like, commenti, share, salvataggi) con diagnosi sullo share in DM
- **Principi algoritmo 2026** integrati

## Deploy su Vercel

1. Crea una **nuova repository** su GitHub e carica questi file (trascinandoli nella UI di GitHub oppure con `git push`).
2. Vai su [vercel.com](https://vercel.com) → **Add New → Project** → importa la repository.
3. Framework Preset: **Other** (è un sito statico, nessun build). Premi **Deploy**.
4. Ottieni un URL stabile, tipo `john-dark-command-center.vercel.app`.

## Usala come app sul telefono

1. Apri l'URL Vercel su **Safari** (iPhone).
2. Tasto **Condividi → Aggiungi alla schermata Home**.
3. Parte a tutto schermo, con icona e nome "John Dark".

## Dati e salvataggio

- I dati (task spuntati, numeri loggati) si salvano in **locale sul dispositivo** (localStorage del browser).
- Sono **per dispositivo e per browser**: i dati del telefono non si sincronizzano con il computer.
- Se cancelli i dati di navigazione del browser, si azzerano.
- Non è un backup nel cloud — per gestire un mese di lancio da telefono è più che sufficiente.

## Struttura

```
index.html              app completa (self-contained)
manifest.webmanifest    config per "Aggiungi a Home" (Android/Chrome)
apple-touch-icon.png    icona home screen iOS
icons/                  icone 192 / 512
README.md
```

## Note

- I contenuti generati (cover/teaser) restano dietro le quinte: l'app non li espone mai.
- Il teaser d'annuncio del 17/06 è già segnato come pubblicato.
