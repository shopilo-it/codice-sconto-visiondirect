# Codice sconto Vision Direct, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Vision Direct** da [shopilo.it](https://shopilo.it/negozi/visiondirect.it). Restituisce **coupon Vision Direct** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-visiondirect](https://shopilo-it.github.io/codice-sconto-visiondirect/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-visiondirect
cd codice-sconto-visiondirect
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Vision Direct",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su lenti a contatto e occhiali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/visiondirect.it"
  }
]
```

## Coupon Vision Direct disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su lenti a contatto e occhiali | [shopilo.it](https://shopilo.it/negozi/visiondirect.it) |

Codici attivi: **[shopilo.it/negozi/visiondirect.it](https://shopilo.it/negozi/visiondirect.it)**

## Domande frequenti

### Come utilizzo un codice sconto Vision Direct?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/visiondirect.it), aggiungi i prodotti al carrello su Vision Direct e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Vision Direct?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Vision Direct piu recenti?
La pagina [shopilo.it/negozi/visiondirect.it](https://shopilo.it/negozi/visiondirect.it) viene aggiornata quotidianamente con i codici sconto Vision Direct, voucher Vision Direct e coupon promozionali Vision Direct piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Vision Direct

Vision Direct e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/visiondirect.it) trovi i migliori codici sconto Vision Direct, coupon Vision Direct verificati e voucher Vision Direct attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-visiondirect
```

```javascript
const { fetchCoupons } = require('codice-sconto-visiondirect');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
