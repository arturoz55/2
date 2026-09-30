# Ducat launch kit

Official account: [@Nodalftech](https://x.com/Nodalftech)
$DUCT contract: `0x263187d5882a7a17f867a8f527c50c6bae7d0a8c` (also shown on the site)

Replace `[website link]` and `[repository link]` before posting. Keep the contract address identical everywhere.

---

## X profile

**Bio, English (160 characters max):**
> Every trade, split smart. ☀️ Split-route swaps and private $ZEC payments. Home of $DUCT, the Ducat community token. Only trust links from this account.

**Bio, short:**
> Every trade, split smart. ☀️ Home of $DUCT.

**Bio, Spanish:**
> Cada trade, dividido con inteligencia. ☀️ Swaps por rutas y pagos privados en $ZEC. Hogar de $DUCT. Solo confía en los enlaces de esta cuenta.

**Other fields**
- Name: `Ducat ☀️` or `Ducat | $DUCT`
- Profile photo: `ducat-x-avatar.png` (400×400)
- Header: `ducat-x-banner-sea.png` (sea, logo and floating cards), `ducat-x-banner.png` or `ducat-x-banner-logo.png` (all 1500×500)
- Website: [website link]
- Pinned post: the launch tweet, then the safety tweet

---

## Images

All tweet images are 1600×900 (16:9, the shape X shows uncropped in the timeline).

| File | Use it with |
|---|---|
| `ducat-launch.mp4` | Launch tweet (16 s video) |
| `ducat-tweet-coin.png` | Launch tweet as a still, or tweet 1 |
| `ducat-tweet-split.png` | Tweet 2 |
| `ducat-tweet-zec.png` | Tweet 3 |
| `ducat-tweet-safety.png` | Tweet 5 (pin it) |
| `ducat-og-image.png` | Link preview when the site is shared |

The split image uses the router simulation's numbers and says so on the image.

---

## Launch tweet (attach `ducat-launch.mp4`)

> Meet Ducat ☀️
>
> A ducat was once the gold coin everyone trusted. $DUCT is ours.
>
> Ducat cuts a big trade into slices, sends each to the venue that prices it best, and settles them in one transaction.
>
> CA: 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c
> [website link]

---

## Tweets

**1. Meet $DUCT** · image: `ducat-tweet-coin.png`
> Merchants once trusted the ducat because it was always the same weight of gold.
>
> We want $DUCT to earn trust the same way: one contract, one site, everything open to read.
>
> Every trade, split smart. ☀️

**2. Why split a trade** · image: `ducat-tweet-split.png`
> One pool gets more expensive the deeper you trade into it.
>
> Ducat splits your order into 5% slices and gives each slice to the venue that returns the most. If a split doesn't beat its own gas, it doesn't happen.

**3. Private ZEC payments** · image: `ducat-tweet-zec.png`
> Get paid in $ZEC without broadcasting it.
>
> Paste your shielded address on Ducat, pick an amount, add a memo, and share the QR code or link. The amount and memo stay encrypted.
>
> [website link]

**4. Price alerts**
> New on Ducat: price alerts. 🔔
>
> Pick a pair, set a price, and Ducat tells you when it crosses. They run on the demo prices for now, and they're ready for live markets.

**5. Safety** · image: `ducat-tweet-safety.png` (pin this)
> Stay safe with $DUCT 🛡️
>
> • The only contract is the one on our site and pinned here.
> • We never DM first.
> • We never ask for your seed phrase.
>
> If someone "from Ducat" messages you, it isn't us.

**6. Open source**
> Ducat's site is open source under the MIT License.
>
> Read the router, check the Zcash address validator, fork it, improve it. Building in public, one slice at a time. ☀️
>
> [repository link]

---

## Article

**Title for X:** Ducat: an old coin's idea of trust, rebuilt for on-chain trading

**Subtitle (optional):** Split-route swaps, private ZEC payments, and what $DUCT is for.

### Why "Ducat"

For centuries the ducat was the coin traders relied on. Its value came from being the same everywhere: the same weight and the same gold, whoever handed it to you. We picked the name because that is the standard we want to hold ourselves to. We aim to be predictable, open and easy to check.

### The problem with one big trade

Automated market makers price along a curve. The first unit you buy from a pool is cheap, and every unit after it costs a little more. On a small trade you barely notice. On a large one, a single pool can cost you several percent in price impact before fees.

Most of that loss is avoidable. Liquidity is spread across many venues, and each can absorb part of an order cheaply. The work is deciding how much to send where.

### How Ducat routes an order

Ducat treats every order as twenty slices of 5% each.

1. **Read every venue.** For the pair you're trading, Ducat looks at each venue's depth and fee tier. Stable-swap pools join only when both tokens are stablecoins.
2. **Give each slice to the best bidder.** Slices go one at a time to whichever venue returns the most for that slice, given what earlier slices already took.
3. **Weigh the gas.** Every extra leg costs gas. Ducat keeps a split only when it beats the best single venue after gas.
4. **Settle together.** All legs execute in one transaction with a minimum-output check. If the market moves further than your slippage setting allows, the whole swap reverts.

On the site, a chart shows how price impact grows with order size for the split route and for the best single venue. In the router simulation, splitting roughly halves the impact across most sizes.

### Privacy with Zcash

Payments shouldn't have to be public to be simple. Ducat builds standard ZIP-321 payment requests: paste your shielded Zcash address, choose an amount and an optional memo, and share the QR code or link. The payer's wallet fills everything in. With a shielded address, the amount, the sender and the memo stay encrypted on chain, and your address never leaves your browser.

When you send ZEC to someone, Ducat checks the address checksum offline, tells you whether it's shielded or transparent, and rejects testnet and retired addresses.

### What $DUCT is

$DUCT is the community token of the Ducat project. The contract address is published on the site and pinned on this account. Those are the only two places to check it.

- Only use the contract address shown on our site.
- Ducat never DMs first and never asks for a seed phrase.
- Crypto is volatile. Nothing here is financial advice.

### What's live today, and what's next

Today you can:

- Try the router with simulated prices and a demo wallet.
- Connect your own wallet (MetaMask, Phantom, Rabby, Coinbase Wallet and more) in read-only mode to see your balances.
- Set price alerts.
- Create private ZEC payment requests.
- Read all of the code under the MIT License.

Next, we're connecting the router to on-chain settlement so that the quote you see becomes a trade you can sign. We'll share progress here as it lands.

Every trade, split smart. ☀️

[website link] · CA: 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c

---

## X article, ready to paste

**Title:** Ducat: trading the way a trusted coin should work

```
For centuries, the ducat was the coin people could count on. Its value came from being the same everywhere: the same weight, the same gold, no matter who handed it to you. We named our project after it because that is the standard we want to be held to.

The problem with one big trade

When you swap on a single pool, every unit you buy costs a little more than the last. On a small trade you barely notice. On a large one, a single pool can cost you several percent in price impact before fees. Most of that loss is avoidable, because liquidity is spread across many venues.

How Ducat routes a trade

Ducat splits every order into twenty slices of 5% each. Each slice goes to the venue that returns the most for it, given what earlier slices already took. A split is kept only when it beats the best single venue after gas. All legs settle together in one transaction, and if the market moves further than your slippage allows, the whole swap reverts instead of filling at a bad price.

In our router simulation, splitting cuts price impact roughly in half across most order sizes. On a 1 million dollar order, that is about 2.6% instead of 5.3%.

Private payments in ZEC

Ducat also builds private payment requests in shielded Zcash. Paste your shielded address, pick an amount, add a memo, and share the QR code or link. With a shielded address, the amount, the sender and the memo stay encrypted, and your address never leaves your browser.

What $DUCT is

$DUCT is the community token of the Ducat project.

Contract: 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c

This contract is published on our site and pinned on this account. Those are the only two places to check it. We never DM first and we never ask for a seed phrase.

What works today

You can try the router with simulated prices and a demo wallet, connect your own wallet in read-only mode, set price alerts, and create private ZEC payment requests. Next, we are connecting the router to on-chain settlement so the quote you see becomes a trade you can sign.

The code is open source under the MIT License.

Crypto is volatile and nothing here is financial advice.

Every trade, split smart.
```

---

## More tweets

**7. The name**
> Why "Ducat"?
>
> For centuries the ducat was the coin traders trusted, because it was the same gold everywhere.
>
> Same idea for $DUCT: one contract, one official site, everything open to read. ☀️

**8. Big orders**
> Big order, one pool = you pay for it in price impact.
>
> Ducat splits it into 20 slices across several venues and settles them together.
>
> In our router simulation: 2.6% impact instead of 5.3% on a $1M order.
>
> $DUCT

**9. Check the contract**
> The only $DUCT contract:
>
> 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c
>
> It's on our site and pinned here. Anything else isn't us. ☀️
