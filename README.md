# Codice sconto Kasanova, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Kasanova** da [shopilo.it](https://shopilo.it/negozi/kasanova.it). Restituisce **coupon Kasanova** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-kasanova](https://shopilo-it.github.io/codice-sconto-kasanova/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-kasanova
cd codice-sconto-kasanova
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Kasanova",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su articoli per la casa",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/kasanova.it"
  }
]
```

## Coupon Kasanova disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su articoli per la casa | [shopilo.it](https://shopilo.it/negozi/kasanova.it) |

Codici attivi: **[shopilo.it/negozi/kasanova.it](https://shopilo.it/negozi/kasanova.it)**

## Domande frequenti

### Come utilizzo un codice sconto Kasanova?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/kasanova.it), aggiungi i prodotti al carrello su Kasanova e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Kasanova?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Kasanova piu recenti?
La pagina [shopilo.it/negozi/kasanova.it](https://shopilo.it/negozi/kasanova.it) viene aggiornata quotidianamente con i codici sconto Kasanova, voucher Kasanova e coupon promozionali Kasanova piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Kasanova

Kasanova e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/kasanova.it) trovi i migliori codici sconto Kasanova, coupon Kasanova verificati e voucher Kasanova attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-kasanova
```

```javascript
const { fetchCoupons } = require('codice-sconto-kasanova');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
