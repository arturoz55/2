# Tessera Swap

A single-page site for a split-route DEX aggregator. It includes a working demo router that splits each order into 5% slices across several liquidity venues.

Open `index.html` in a browser. It needs no build step and has no dependencies other than Google Fonts.

## What works

- Swap widget: token picker with search and keyboard navigation, flip, MAX, input sanitizing, a rate you can invert, and a details panel (price impact, minimum received, network fee).
- Router: greedy constant-product slicing across 5 venues (at most 4 legs). A split is kept only when it beats the best single venue after gas. Stable-swap venues are used only for stable-to-stable pairs.
- Live quotes: prices drift every 12 seconds, shown on a countdown ring. You can also refresh manually.
- Settings: slippage presets or a custom value (validated to 0.01–50%) and a transaction deadline.
- Demo wallet: simulated balances, a review dialog, a pending state, and settlement that reverts when the output falls below the minimum. Includes an activity list, disconnect, and toasts.
- Hero: a night sky painted in code on a canvas (stars, a milky band, drifting clouds, trees) with a grid overlay. It respects reduced motion.
- Price chart for the selected pair (1H/1D/1W/1M, hover tooltip, invert) and a markets list with 24h sparklines and filters. Click a market to pay with that token.
- Route presets (1 / 25 / 250 / 1,500 ETH), 25% / 50% / MAX buttons, copy quote, reset settings, account holdings, reset balances, expand-all FAQ, back-to-top, section-aware nav, and a `/` shortcut to the amount field.
- Light and dark themes and a mobile nav.

**Demo only.** No real wallet or on-chain transactions. Going live would need an aggregator API or router contract.

## Zcash

- **ZEC tips.** The "Tip in ZEC" section builds a [ZIP-321](https://zips.z.cash/zip-0321) payment request (`zcash:<address>?amount=…&memo=…`) with a QR code, amount presets, an encrypted memo (512 bytes max), copy buttons and an "Open in Zcash wallet" link.
  **To turn tips on,** paste your shielded address (starting `u1…` or `zs1…`) into `data-zcash-address` on `<section id="tips">` in `index.html`. Until then, the section shows a setup notice.
- **Send ZEC to an address.** In the swap card, "Send to another address" accepts a Zcash address when the receive token is ZEC. It checks the address offline:
  - Unified and TEX addresses: Bech32m checksum.
  - Sapling addresses: Bech32 checksum.
  - Transparent `t1`/`t3` addresses: Base58Check checksum.

  It rejects testnet and Sprout addresses and labels each address as shielded or transparent. The encrypted memo field appears only for shielded addresses.
- ZEC is in the token list, the markets panel and the price ticker.

## License

MIT. See [LICENSE](LICENSE).
