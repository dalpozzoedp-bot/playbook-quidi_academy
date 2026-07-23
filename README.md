# Playbook dell'ascolto — Quindi Academy

Pagina web autonoma del playbook. Nessuna dipendenza da installare:
si apre direttamente con doppio clic su `index.html`.

## Struttura

```
playbook-web/
├── index.html      → tutto il testo del playbook
├── css/style.css   → colori, font, impaginazione
├── js/main.js      → barra di avanzamento lettura
└── README.md
```

## Come modificarlo

**Cambiare il testo** → `index.html`. Ogni sezione è racchiusa in un
blocco `<section class="sec" id="...">` con un commento sopra che la
identifica (es. `<!-- 04 OSSERVARE CHI PARLA -->`).

**Cambiare i colori** → `css/style.css`, in cima nel blocco `:root`.
Sono sei variabili con il nome del colore accanto; cambiando il valore
lì si aggiorna tutta la pagina.

**Aggiungere una citazione** → copia un blocco `<blockquote class="quote">`
esistente e sostituisci testo e autore.

**Aggiungere una riga alla tabella Sì/No** → cerca `<div class="yesno">`
e aggiungi un `<li>` nella colonna giusta.

## Anteprima in VS Code

Con l'estensione **Live Server**: tasto destro su `index.html` →
"Open with Live Server". Le modifiche si aggiornano da sole nel browser.
Senza estensione, basta aprire il file nel browser e ricaricare.

## Condividerlo

- **Cartella zippata** via email o chat.
- **Stampa/PDF**: dal browser, Stampa → Salva come PDF (il foglio di
  stile ha già le regole per la stampa).
- **Link**: caricando la cartella su un hosting statico
  (GitHub Pages, Netlify) si ottiene un URL condivisibile.
