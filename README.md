# Home Internet Plan Selection: Clickable Prototype

A mobile-first, clickable HTML prototype of a home internet checkout flow, rebuilt from my Figma case study. Part of my portfolio: [abhishekbora.myportfolio.com](https://abhishekbora.myportfolio.com).

> **Portfolio prototype, not a real store.** No orders are placed and no data is collected. Brand names and logos have been replaced with a neutral placeholder ("Acme").

## The flow

| Step | Screen | What you can do |
|---|---|---|
| 1 | **Select your plan** | Tap a plan card to expand it, toggle the AutoPay discount (prices update live), pick 1 additional gift, **Add to cart** |
| 2 | **Enhance your services** (add-ons hub) | Everything here is optional. Shop Perks, Live TV or Home Phone, or skip straight to **Review & checkout** |
| 2a | Popular perks | Add or remove streaming perks |
| 2b | Explore Live TV | Expand a TV plan and add it (one at a time) |
| 2c | Home Phone | Select and continue (returns to the hub) |
| 3 | **Review your order** | See everything in the cart, remove add-ons, apply the online offer, **Proceed to payment** (end of prototype) |

The **monthly total** stays in a sticky tray at the bottom of every screen and updates as you change the order. The cart icon shows how many items you have.

## Built with

- A single `index.html`: plain HTML, CSS and JavaScript. No framework, no build step.
- **Inter** and **Material Symbols Outlined**, loaded from Google Fonts.
- Hash-based routing (`#plan`, `#services`, `#perks`, `#tv`, `#phone`, `#review`), so the browser back button works and it runs on GitHub Pages as-is.
- Design tokens (colours, radii, type sizes, spacing) taken directly from the Figma frames.

## Differences from the Figma file

- The Verizon logo, name, phone number and "Fios" product names are replaced with the placeholder brand **Acme**. Partner logos (streaming services, gift cards, the router photo) are drawn as neutral CSS tiles.
- The Review screen in Figma was a flattened screenshot. It is rebuilt here as live HTML.
- The steps tracker highlights **Services** on the add-ons hub. The Figma frame highlights "Plan" there.
- Added to make the prototype interactive: the sticky total tray on the plan and review screens, "Added" states, "Remove" links on the review screen, the third gift option, and the end-of-prototype sheet.

## Run it locally

Open `index.html` in any browser. That's all. To test on a phone on the same Wi-Fi, run `python3 -m http.server 8000` in this folder and visit `http://<your-computer-ip>:8000`.

## Credits

UX and UI design: Abhishek Bora. Figma source: *Figma basics → Verizon home trans* (frames 2380:10092, 2380:9344, 2380:9681 and the "final design" flow).
