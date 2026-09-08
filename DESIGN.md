<!-- Design decision for the Wix-faithful Newport Sailing rebuild.
     Business: Newport Sailing School and Tours -->

# DESIGN.md — Newport Sailing School and Tours

archetype: classic-nautical-local
rationale: Exact-design replica of newportsailing.com. Fifty-plus years of family ownership, ASA certification, and a harbor-first product line call for a classic New England sailing look — Rozha One display type, warm cream bands, brick-red pill CTAs, and full-bleed harbor photography — rather than a generic upscale template.
interaction_level: L2

personality: [welcoming, adventurous, trustworthy, local_expert]

typography:
  display: "Rozha One"
  body: "Jost"
  scale: 1.250
  notes: "Rozha One for ALL headings and primary nav links (Wix source used Rozha One site-wide for chrome). Jost is the free stand-in for Wix's proprietary Avenir. Hero h1 uses clamp(2.9rem, 7vw, 4.7rem); section h2 uses clamp(2rem, 4.5vw, 2.8rem); body ~1.08–1.14rem / 1.7 line-height. Eyebrows are Jost uppercase with letter-spacing 0.2em."

palette:
  primary: "#1b3a5b"
  secondary: "#efe9e6"
  accent: "#aa2b2b"
  application: "Primary navy appears in logo chrome accents and text links. Secondary cream (#efe9e6) is the soft section ground and footer. Accent brick-red (#aa2b2b) is reserved for pill CTAs (border-radius 100px) and underline accents on nav hover/active. Hero overlay uses #233c6d. Heading ink is near-black #282828; body ink #33383d."

composition:
  whitespace: balanced
  photography: dominant
  card_usage: interaction-only
  mobile: "Below 1120px the desktop nav collapses to a hamburger; drawer slides from the right over a scrim. Feature/testimonial grids drop to 2 then 1 column. Split and contact layouts stack. Gallery masonry columns: 3 → 2 → 1."

shell:
  header: |
    Sticky white header, min-height ~108px. Logo left (~96px wide) linking to index.html.
    Desktop nav right-aligned in Rozha One ~1.32rem: Home · Services (dropdown) · About Us · Gallery · Reviews · Online Booking · Contact, with brick-red underline on hover/active.
    Services dropdown lists Sailing Tours, Sailing Instruction, Team Building, Custom Sailing Experiences, plus View all services.
    Mobile: hamburger opens a right drawer with the same links and a Book Online CTA.
  nav: ["Home", "Services", "About Us", "Gallery", "Reviews", "Online Booking", "Contact"]
  footer: |
    Cream (#efe9e6) footer with top border. Four columns on desktop: brand + tagline, Explore links, Set Sail contact (address / phone / email / hours), then bottom legal row with © year, Privacy, Terms, Contact.
    Free-parking note sits above the legal row.

pages:
  - slug: index
    title: "Newport Sailing School and Tours | Sailing Tours & Lessons in Newport, RI"
    h1: "Newport Sailing School & Tours"
    intent: "Land visitors, prove trust, and push FareHarbor booking."

  - slug: services
    title: "Sailing Services | Newport Sailing School and Tours"
    h1: "Our Sailing Services"
    intent: "Overview of tours, instruction, team building, and custom sails."

  - slug: sailing-tours
    title: "Sailing Tours | Newport Sailing School and Tours"
    h1: "Sailing Tours"
    intent: "Narrated harbor / bay tours with rates and Book CTA."

  - slug: sailing-instruction
    title: "Sailing Instruction | Newport Sailing School and Tours"
    h1: "Sailing Instruction"
    intent: "ASA courses and certification path."

  - slug: team-building
    title: "Team Building | Newport Sailing School and Tours"
    h1: "Team Building"
    intent: "Corporate charters and group sailing events."

  - slug: custom-sailing
    title: "Custom Sailing Experiences | Newport Sailing School and Tours"
    h1: "Custom Sailing Experiences"
    intent: "Private occasions — engagements, celebrations, family outings."

  - slug: about
    title: "About Us | Newport Sailing School and Tours"
    h1: "About Us"
    intent: "Family story since 1965 / 1971 and crew trust."

  - slug: gallery
    title: "Gallery | Newport Sailing School and Tours"
    h1: "Gallery"
    intent: "Photo proof of life on the water."

  - slug: reviews
    title: "Reviews | Newport Sailing School and Tours"
    h1: "Reviews"
    intent: "Customer testimonials."

  - slug: booking
    title: "Online Booking | Newport Sailing School and Tours"
    h1: "Online Booking"
    intent: "Embedded FareHarbor calendar."

  - slug: contact
    title: "Contact | Newport Sailing School and Tours"
    h1: "Contact"
    intent: "NAP, map, and Kora contact form."

  - slug: privacy
    title: "Privacy Policy | Newport Sailing School and Tours"
    intent: "Legal."

  - slug: terms
    title: "Terms & Conditions | Newport Sailing School and Tours"
    intent: "Legal."

  - slug: "404"
    title: "Page Not Found | Newport Sailing School and Tours"
    intent: "Fallback."

sections:
  - id: hero
    layout: full-bleed-image
    show: home
    spec: "Full-bleed lighthouse / harbor hero, centered white Rozha One headline, Jost tagline, stacked pill CTAs (Book Online Now + secondary), phone/email block, ASA badge lower-right."

  - id: features
    layout: three-up
    show: home
    spec: "Three plain feature columns (no card chrome) highlighting tours, instruction, and private experiences."

  - id: story
    layout: split
    show: home / about
    spec: "Image + copy split; cream or white alternating bands."

  - id: offerings
    layout: service-cards
    show: home / services
    spec: "2×2 service cards with image, short copy, and accent CTA linking to detail pages."

  - id: reviews
    layout: testimonial-grid
    show: home / reviews
    spec: "Three-up review cards with stars and serif attribution."

  - id: gallery
    layout: masonry
    show: gallery
    spec: "True masonry (column-count), natural aspect ratios, no crop."

  - id: contact
    layout: form-aside
    show: contact
    spec: "Two-column contact form + cream aside with NAP; form POSTs to Kora public forms API."

  - id: booking
    layout: embed
    show: booking
    spec: "FareHarbor iframe in a bordered frame."

avoid:
  - Replacing Rozha One nav/headings with Inter or another sans
  - Sharp 4px CTA corners (source uses pill / 100px radius)
  - Dark navy footer (source footer is cream)
  - Stock photography or Wix CDN hotlinks
  - Auto-advancing carousels
  - Purple/indigo AI-default themes
