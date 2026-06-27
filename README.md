# BidFTA Fee Calculator

I bid $5.50 on a rug. I paid $8.01. I built a calculator.

That's the whole origin story.

**[Try it here →](https://alsoadarsh.github.io/bidfta-calculator)**

> Works on any browser. Install it on your phone like an app — no App Store needed.

---

## What it does

BidFTA stacks fees in a way that turns a "great deal" into a "wait, how much?" moment at checkout. This calculator shows you the real number before you commit — and a few things beyond that.

**Auction mode**
Enter your bid → get the actual charge. Covers the 17.25% buyer's premium, freight surcharge ($1.00 for items ≥ $5, $0.25 for items under $5), and 7.5% sales tax. No surprises.

**Bins mode**
Simpler. Just the price plus tax. No premium, no freight.

**Reverse calculator**
Have a hard budget? Enter your max spend and it works backwards to tell you the highest bid you can safely place. Useful when you're determined not to go over $40 on a blender you don't need.

**BidFTA link auto-fill**
Paste a BidFTA item link and it pulls the item name, current bid price, and MSRP directly from BidFTA's API. No typing, no copying. Just paste and go.

**Deal comparison**
Enter what the same item sells for on Amazon, Walmart, or wherever. Hit the Search Amazon button and it opens a search in a new tab so you can grab the price quickly. The calculator then tells you whether you're actually saving money — and flags the no-warranty situation when the savings are slim.

**Session tally**
Watching multiple lots in one session? Add items as you go and track your total spend before the auctions end. Each item stores the full fee breakdown — tap to expand. The grand total updates live.

**Dark / light mode**
Because sometimes the good deals happen at midnight.

---

## Install it on your phone

This is a PWA (Progressive Web App) — it installs directly from the browser, no App Store required.

**Android (Chrome)**
Visit the link → tap the three-dot menu → "Add to Home Screen"

**iPhone (Safari)**
Visit the link → tap the Share button → "Add to Home Screen"

Once installed it gets its own icon, runs fullscreen, and works offline.

---

## Why this exists

I shop BidFTA regularly. The fee math isn't complicated, but doing it in your head mid-auction — on your phone, while the countdown ticks — is annoying enough that I kept getting it wrong. Now I don't.

It's a personal tool. I made it public in case anyone else finds it useful. If the fees change and I haven't updated it yet, feel free to open an issue.

---

## Fee reference

| Fee | Amount |
|---|---|
| Buyer's Premium | 17.25% of bid |
| Freight (bid ≥ $5) | $1.00 flat |
| Freight (bid < $5) | $0.25 flat |
| Sales Tax | 7.5% of subtotal |

Fees can change. Always verify at [bidfta.com](https://bidfta.com) before trusting any calculator, including this one.

---

## Tech

Vanilla HTML, CSS, and JavaScript. No frameworks, no npm, no build step, no backend.

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.json` | Makes it installable as a PWA |
| `sw.js` | Service worker — handles offline caching |
| `icon-192.png` | App icon |
| `icon-512.png` | App icon (large, for splash screens) |

Item data (name, current bid, MSRP) is pulled from BidFTA's API. Everything else runs locally in the browser. No data is collected or stored anywhere.

---

*Personal project. Not affiliated with or endorsed by BidFTA.*
