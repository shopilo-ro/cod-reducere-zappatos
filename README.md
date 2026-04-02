# Cod reducere Zappatos — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Zappatos** de pe [shopilo.ro](https://shopilo.ro/magazin/zappatos.ro). Returneaza **cupoane Zappatos** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-zappatos](https://shopilo-ro.github.io/cod-reducere-zappatos/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-zappatos
cd cod-reducere-zappatos
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Zappatos",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% reducere la produse nou adaugate",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/zappatos.ro"
  }
]
```

## Cupoane Zappatos disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% reducere la produse nou adaugate | [shopilo.ro](https://shopilo.ro/magazin/zappatos.ro) |

Codurile active: **[shopilo.ro/magazin/zappatos.ro](https://shopilo.ro/magazin/zappatos.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Zappatos?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/zappatos.ro), adauga produsele in cos pe Zappatos, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Zappatos?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Zappatos?
Pagina [shopilo.ro/magazin/zappatos.ro](https://shopilo.ro/magazin/zappatos.ro) este actualizata zilnic cu cele mai noi cod reducere Zappatos, voucher Zappatos si cupon promotional Zappatos.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Zappatos

Zappatos este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/zappatos.ro) cele mai bune cod reducere Zappatos, cupoane Zappatos verificate si voucher Zappatos active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-zappatos
```

```javascript
const { fetchCoupons } = require('cod-reducere-zappatos');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
