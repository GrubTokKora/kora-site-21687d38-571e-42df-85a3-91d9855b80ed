## index.html → /
title: Newport Sailing School and Tours | Sailing Tours &amp; Lessons in Newport, RI
purpose: Landing page with hero booking CTA, feature highlights, story, service overview, reviews, FAQ, and location details.
contains:
- `#hero` — Full-bleed harbor hero, Book Online Now, phone/email, ASA badge
- features — Three-up plain columns (tours / instruction / private)
- story / about band — Family-owned since 1965 copy with media
- services overview — Cards linking to detail pages
- reviews — Testimonial grid
- FAQ — Visible accordion + FAQPage JSON-LD
- hours / location — Address, map link, parking note
also: FareHarbor lightframe script is loaded site-wide for Book CTAs. Header and footer are static in the HTML (not JS-injected) for crawlers.

## services.html → /services
title: Sailing Services | Newport Sailing School and Tours
purpose: Overview of all four service lines with links to detail pages.

## sailing-tours.html → /sailing-tours
title: Sailing Tours | Newport Sailing School and Tours
purpose: Narrated Newport Harbor / Narragansett Bay tours, rates, and booking CTA.

## sailing-instruction.html → /sailing-instruction
title: Sailing Instruction | Newport Sailing School and Tours
purpose: ASA-certified sailing courses and certification path.

## team-building.html → /team-building
title: Team Building | Newport Sailing School and Tours
purpose: Corporate charters and team sailing events.

## custom-sailing.html → /custom-sailing
title: Custom Sailing Experiences | Newport Sailing School and Tours
purpose: Private custom sails for special occasions.

## about.html → /about
title: About Us | Newport Sailing School and Tours
purpose: Company story, family ownership, and crew trust.

## gallery.html → /gallery
title: Gallery | Newport Sailing School and Tours
purpose: Masonry photo gallery of life on the water.

## reviews.html → /reviews
title: Reviews | Newport Sailing School and Tours
purpose: Customer testimonials grid.

## booking.html → /booking
title: Online Booking | Newport Sailing School and Tours
purpose: Embedded FareHarbor booking calendar.

## contact.html → /contact
title: Contact | Newport Sailing School and Tours
purpose: NAP, map, hours, and Kora public contact form (reCAPTCHA slot).

## privacy.html → /privacy
title: Privacy Policy | Newport Sailing School and Tours
purpose: Privacy policy prose.

## terms.html → /terms
title: Terms &amp; Conditions | Newport Sailing School and Tours
purpose: Terms and conditions prose.

## 404.html → /404
title: Page Not Found | Newport Sailing School and Tours
purpose: Fallback not-found page with path back home / contact.

## shared (every page)
Sticky header with Services dropdown, mobile drawer, cream footer, `assets/styles.css` (compiled from `src/input.css`), `js/includes.js` (nav behaviour), and `js/main.js` (forms, year, FareHarbor helpers). `window.KORA_SITE_CONFIG` / `KORA_CONFIG` present on every page.
