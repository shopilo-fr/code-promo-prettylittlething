# Code promo PrettyLittleThing, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo PrettyLittleThing** depuis [shopilo.fr](https://shopilo.fr/reductions/prettylittlething.fr). Renvoie les **coupons PrettyLittleThing** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-prettylittlething](https://shopilo-fr.github.io/code-promo-prettylittlething/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-prettylittlething
cd code-promo-prettylittlething
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "PrettyLittleThing",
    "code": "SHOPILO25",
    "discount": "25%",
    "description": "25% de reduction sur toute la collection",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/prettylittlething.fr"
  }
]
```

## Coupons PrettyLittleThing disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 25% | 25% de reduction sur toute la collection | [shopilo.fr](https://shopilo.fr/reductions/prettylittlething.fr) |

Codes actifs : **[shopilo.fr/reductions/prettylittlething.fr](https://shopilo.fr/reductions/prettylittlething.fr)**

## Questions frequentes

### Comment utiliser un code promo PrettyLittleThing ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/prettylittlething.fr), ajoutez les produits a votre panier sur PrettyLittleThing et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons PrettyLittleThing ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction PrettyLittleThing les plus recents ?
La page [shopilo.fr/reductions/prettylittlething.fr](https://shopilo.fr/reductions/prettylittlething.fr) est mise a jour quotidiennement avec les codes promo PrettyLittleThing, bons de reduction PrettyLittleThing et coupons promotionnels PrettyLittleThing les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de PrettyLittleThing

PrettyLittleThing est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/prettylittlething.fr), retrouvez les meilleurs codes promo PrettyLittleThing, coupons PrettyLittleThing verifies et bons de reduction PrettyLittleThing actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-prettylittlething
```

```javascript
const { fetchCoupons } = require('code-promo-prettylittlething');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
