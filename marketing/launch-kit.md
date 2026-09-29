# Florin launch kit

Official account: [@Nodalftech](https://x.com/Nodalftech). The site links to it from the entry page, the header and the footer, and "Share on X" posts credit it with `via @Nodalftech`.

$FLRN contract: `0x263187d5882a7a17f867a8f527c50c6bae7d0a8c` (also shown on the site). Replace the remaining `[brackets]` before posting.

---

## X bio (160 characters max)

**Main (English):**
> Split-route swaps that cut every trade into its best pieces. Private payments in shielded $ZEC. Home of $FLRN. Only trust links from this account. 🌙

**Short (English):**
> Every trade, split smart. 🌙 Split-route swaps + private $ZEC payments. Home of $FLRN.

**Spanish:**
> Swaps que dividen cada trade en sus mejores partes. Pagos privados en $ZEC blindado. Hogar de $FLRN. Solo confía en los enlaces de esta cuenta. 🌙

**Other profile fields**
- Name: `Florin 🌙` or `Florin | $FLRN`
- Handle: @Nodalftech
- Header: `nodal-x-banner.png` or `nodal-x-banner-logo.png` (1500×500)
- Website: [website link]
- Pinned post: the launch tweet

---

## Images

All 1600×900 (16:9, the shape X shows uncropped in the timeline): `nodal-tweet-ndl.png`, `nodal-tweet-split.png`, `nodal-tweet-zec.png`, `nodal-tweet-safety.png`. The split image uses the router simulation's numbers and says so on the image.

---

## Launch tweet (attach `nodal-launch.mp4`, or `nodal-tweet-ndl.png` for a still post)

> Meet Florin 🌙
>
> It cuts a big trade into slices, sends each slice to the venue that prices it best, and settles everything in one transaction.
>
> Try the router demo. Request $ZEC privately. $FLRN is here.
>
> CA: 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c
> [website link]

---

## Tweets

**1. Why split a trade** · image: `nodal-tweet-split.png`
> One pool gets more expensive the deeper you trade into it.
>
> Florin splits your order into 5% slices and gives each slice to the venue that returns the most for it. If a split doesn't beat its own gas, it doesn't happen.
>
> Every trade, split smart. $FLRN

**2. Private ZEC payment requests** · image: `nodal-tweet-zec.png`
> Get paid in $ZEC without broadcasting it.
>
> Paste your shielded address on Florin, pick an amount, add a memo, and share the QR code or link. The payer's wallet fills in the rest, and the amount and memo stay encrypted.
>
> [website link]

**3. Address checks**
> Pasting a Zcash address into Florin?
>
> It checks the checksum before you send, tells you whether the address is shielded (u1…, zs1…) or transparent (t1…), and rejects testnet addresses.
>
> One typo shouldn't cost you a transfer.

**4. Safety** · image: `nodal-tweet-safety.png` (pin this one too)
> Safety first 🛡️
>
> • The only $FLRN contract is the one on our site and pinned here.
> • We never DM first.
> • We never ask for a seed phrase.
>
> If someone "from Florin" messages you, it isn't us.

**5. Open source**
> Florin's site is open source under the MIT License.
>
> Read the router, check the address validator, fork it, improve it. Building in public, one slice at a time. 🌙
>
> [repository link]

**6. Community**
> Night shift at Florin 🌙
>
> What should the router support next: more venues, more chains, or limit orders?
>
> Reply below. $FLRN holders help shape what we build.

---

## Article

**Title for X:** Florin: cutting every trade into its best pieces

**Subtitle (optional):** Split-route swaps, private ZEC tips, and what $FLRN is for.

### The problem with one big trade

Automated market makers price along a curve. The first unit you buy from a pool is cheap, and every unit after it costs a little more. On a small trade you barely notice. On a large one, a single pool can cost you several percent in price impact before fees.

Most of that loss is avoidable. Liquidity is spread across many venues, and each one can absorb part of an order cheaply. The trick is deciding how much to send where.

### How Florin routes an order

Florin treats every order as twenty slices of 5% each.

1. **Read every venue.** For the pair you're trading, Florin looks at each venue's depth and fee tier. Stable-swap pools join only when both tokens are stablecoins.
2. **Give each slice to the best bidder.** Slices go one at a time to whichever venue returns the most for that slice, given what earlier slices already took. Deep venues get more slices, and shallow ones fill up fast.
3. **Weigh the gas.** Every extra leg costs gas. Florin compares the split route with the best single venue after gas and keeps the split only when it actually wins.
4. **Settle together.** All legs execute in one transaction with a minimum-output check. If the market moves further than your slippage setting allows, the whole swap reverts instead of filling at a bad price.

You can watch this happen on the site. Enter a large order and the live route panel shows each leg, its share and the amount it returns.

### Privacy with Zcash

Payments shouldn't have to be public to be simple. So Florin includes private ZEC payment requests.

Paste your shielded Zcash address, choose an amount and add an optional memo. Florin builds a standard ZIP-321 payment request (the Zcash payment link format) and shows it as a QR code and a link you can share. The payer's wallet reads it and fills everything in. Because the address is shielded, the amount, the sender and the memo stay encrypted on chain. Your address never leaves your browser.

At launch, the same section also lets anyone tip the Florin builders in shielded ZEC.

The same care goes into sending. When you send ZEC to an address, Florin verifies the checksum offline and tells you whether it's shielded or transparent. It rejects testnet and retired Sprout addresses, and it offers an encrypted memo only when the recipient can read one.

### What $FLRN is

$FLRN is the community token of the Florin project. The contract address is published on the Florin site and pinned on this account. Those are the only two places to check it.

Please be careful:

- Only use the contract address shown on our site.
- Florin never DMs first and never asks for a seed phrase.
- Crypto is volatile. Nothing here is financial advice.

### What's live today, and what's next

Today you can:

- Try the router with simulated prices and a demo wallet.
- Connect your own wallet (MetaMask, Phantom, Rabby, Coinbase Wallet and more) in read-only mode to see your balances.
- Create private ZEC payment requests with a QR code.
- Read all of the code under the MIT License.

Next, we're connecting the router to on-chain settlement so that the quote you see becomes a trade you can sign. We'll share progress here as it lands.

### Open by default

Florin's site is open source under the MIT License. Read the router, check the address validator, and tell us where it could be better.

Every trade, split smart. 🌙

[website link] · CA: 0x263187d5882a7a17f867a8f527c50c6bae7d0a8c
