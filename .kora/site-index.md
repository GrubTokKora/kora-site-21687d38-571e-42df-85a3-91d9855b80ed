## index.html → /
title: Newport Sailing School and Tours – Sailing Tours &amp; Lessons in Newport, RI
purpose: Landing page featuring company overview, featured offerings, story, photo gallery, customer reviews, location details, and contact info.
contains:
- `#hero` — Hero banner with headline, subtitle, and booking call to action
- "Our Sailing Services" `#offerings` — Priced items and service descriptions grouped by category
- "Newport's First and Only Pure Sailing Tour" `#story` — Company history and background information
- "Life on the Water" `#gallery` — Photo gallery filmstrip and link
- `#reviews` — Featured pull quote and customer review blocks
- `#hours_location` — Location address, parking details, phone, email, and booking button
- `#contact` — Closing call to action band with phone, email, and message link
also: The FAQPage structured data block holds six questions and answers that have no visible counterpart rendered on the screen. The offerings section renders priced instruction items while team building and custom experiences are rendered as paragraphs with no priced items.

## gallery.html → /gallery
title: Photo Gallery — Newport Sailing School and Tours
purpose: Display a photo gallery of sailing tours and boats.
contains:
- "Gallery" — Page intro
- "Life on the Water" — Scrollable photo filmstrip
- "Browse the Full Collection" — Grid of photo items
- "Ready to Experience Newport Under Sail?" — Closing call to action band

## services.html → /services
title: Sailing Tours, Lessons &amp; Team Building — Newport Sailing School
purpose: Present the sailing tours, instruction courses, team building events, and custom sailing experiences with pricing and details.
contains:
- "Our Sailing Services" — introductory hero copy and booking call-to-action
- "Everything We Sail" `#offerings-heading` — overview grid of all service categories and priced items
- "Newport Harbor & Narragansett Bay" `#tours-detail-heading` — detailed sailing tours, descriptions, schedules, and priced items
- "Learn to Sail in Newport, RI" `#instruction-heading` — sailing courses, curriculum list, pricing, and details
- "Set Sail for Your Next Corporate Adventure" `#team-heading` — team building and corporate charter information
- "A Sailing Adventure Created Just for You" `#custom-heading` — custom private sailing experience and occasion tags
- closing call-to-action band
also: The structured-data item list duplicates the sailing tours, sailing instruction, team building, and custom sailing experience offered on the page. The four service offerings appear twice on the page: first in an overview grid under "Everything We Sail", and then expanded into individual detail sections further down.

## shared (every page)
The header, navigation, mobile menu and footer are propagated from index.html to every other page by
`shell_propagation`. A change to any of them is made on index.html alone and copied automatically.
