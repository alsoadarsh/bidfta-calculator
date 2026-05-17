# BidFTA Fee Calculator

I bid $5.50 on a rug. I paid $8.01. I built a calculator.

That's the whole origin story.

**[Try it here →](https://alsoadarsh.github.io/bidfta-calculator)**

---

## What it does

BidFTA stacks fees in a way that turns a "great deal" into a "wait, how much?" moment at checkout. This calculator shows you the real number before you commit.

**Auction mode**
Enter your bid → get the actual charge. Covers the 17.25% buyer's premium, freight surcharge ($1.00 for items ≥ $5, $0.25 for items under $5), and 7.5% sales tax. No surprises.

**Bins mode**
Simpler. Just the price plus tax. No premium, no freight.

**Reverse calculator**
Have a hard budget? Enter your max spend and it works backwards to tell you the highest bid you can safely place. Useful when you're determined not to go over $40 on a blender you don't need.

**Deal comparison**
Paste in the MSRP from the listing and/or what the same item goes for on Amazon or wherever. It tells you whether you're actually saving money — and reminds you there's no warranty, which matters more than people think when the savings are slim.

**Session tally**
Watching multiple lots? Add items as you go and track your total exposure for the session. Each item stores the full fee breakdown — tap to expand. Because sometimes you need to see exactly how many fees you're paying on that $3 lot.

You can paste a BidFTA item link too. It won't auto-fill the name (their URLs are just numbers, unfortunately) but it saves the link so you can jump back to the listing.

**Dark / light mode**
Because sometimes the good deals happen at midnight.

---

## Why this exists

I shop BidFTA regularly. The fee math isn't complicated, but doing it in your head mid-auction — on your phone, while the countdown ticks — is annoying enough that I kept getting it wrong. Now I don't.

It's a personal tool. I made it public in case anyone else finds it useful. If the fees change and I haven't updated it yet, feel free to open an issue.

---

## Usage

**Option 1 —** Use the [live version](https://yourusername.github.io/bidfta-calculator). Nothing to install, works on your phone.

**Option 2 —** Download `index.html` and open it in any browser. Still nothing to install.

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

Single HTML file. Vanilla JS. No dependencies, no npm install, no build step, no backend. Just open it.

---

*Personal project. Not affiliated with or endorsed by BidFTA.*
