# Jupiter

Jupiter API can be used as a pricing source inside Arcana strategies. `Strategy` authors are provided with the `JupiterPricingSource` bean for this functionality. Jupiter's v4 API is used.

---

The primary call, `JupiterPricingSource.getUsdcPriceForSymbol` receives as input:
- ids
- vsAmount

`ids` can be a symbol string, or token mint pubkey.
`vsAmount` is the amount of USDC being priced.

---
```
// https://price.jup.ag/v4/price?ids=ORCA&vsAmount=300
// https://price.jup.ag/v4/price?ids=DezXAZ8z7PnrnRJjz3wXBoRgixCa6xjnB7YaB1pPB263&vsAmount=1500
```