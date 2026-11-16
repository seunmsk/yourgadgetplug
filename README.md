# YourGadgetPlug

Website for YourGadgetPlug, a Lagos store selling phones (brand new and UK used), gadgets and limited timepieces.

**Plug in. Power up. Live better.** · 0909 881 6496 · 0912 931 5752

## What's on the site
- **Hero promo:** buy any iPhone 16–18 Pro Max and get a Bose speaker or 30,000mAh power bank free
- **Phones:** brand new and UK used (battery health 85–100%), with filters, sorting and WhatsApp ordering
- **Compare:** pick two phones and see them side by side, including new vs UK used
- **Gadgets:** speakers, power banks and accessories
- **Limited Timepieces:** one-of-one watches

## Updating stock
All products live in `products.json`. To change stock on GitHub:

1. Open `products.json` and click the ✏️ pencil icon.
2. Change a `price`, set `"inStock": false` to mark an item sold out, or copy an existing item to add a new one.
3. Click **Commit changes**. The site updates on its next deploy.

Product fields:
- `cat`: `phone`, `speaker`, `powerbank`, `accessory` or `watch`
- `cond`: `new` or `uk` (phones only)
- `battery`: battery health for UK-used phones, e.g. `"92%"`
- `promo`: `true` if the phone qualifies for the free gift
- `img`: a photo path such as `img/my-photo.jpg` (upload the photo into the `img` folder)

## Hosting
This is a static site with no build step. Turn on **GitHub Pages** (Settings → Pages → deploy from `main`) or import the repo into Vercel or Netlify.
