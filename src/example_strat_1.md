# Example strategy

This is an example SPL/USDC OpenBook trading strategy, that will match for any generic SPL. In this instance, mSOL is the base token. USDC is the quote token.

---

## Trading Logic (mSOL/USDC)

1. Get top of book bid, top of book ask
2. Calculate % change with our spread applied
3. If price change % is not significant enough from step 2, abort.
4. If price change % is significant enough, after applying our spread, send an order.
5. The order will be a "replace order" only if an existing order is present.