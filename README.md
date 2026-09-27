# Tessera Swap

A single-page site for a split-route DEX aggregator. It includes a working demo router that splits each order into 5% slices across several liquidity venues.

Open `index.html` in a browser. It needs no build step and has no dependencies other than Google Fonts.

## What works

- Swap widget: token picker with search and keyboard navigation, flip, MAX, input sanitizing, a rate you can invert, and a details panel (price impact, minimum received, network fee).
- Router: greedy constant-product slicing across 5 venues (at most 4 legs). A split is kept only when it beats the best single venue after gas. Stable-swap venues are used only for stable-to-stable pairs.
- Live quotes: prices drift every 12 seconds, shown on a countdown ring. You can also refresh manually.
- Settings: slippage presets or a custom value (validated to 0.01–50%) and a transaction deadline.
- Demo wallet: simulated balances, a review dialog, a pending state, and settlement that reverts when the output falls below the minimum. Includes an activity list, disconnect, and toasts.
- Light and dark themes, an animated mosaic canvas (which respects reduced motion), and a mobile nav.

**Demo only.** No real wallet or on-chain transactions. Going live would need an aggregator API or router contract.

## License

MIT. See [LICENSE](LICENSE).
