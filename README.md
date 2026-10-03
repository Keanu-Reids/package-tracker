# Package Tracker

A single-page tracker for Reid Williams. Open `index.html` in a browser (no server, no build).

Add a tracking number and an optional nickname. The page guesses the carrier: UPS when the number starts with `1Z`; USPS for 20–22 digits, a 13-character code ending in `US`, or a long number starting with 94, 93, 92, or 91; FedEx for 12-, 15-, or 22-digit numbers that are not already USPS. If the number does not match, pick FedEx, UPS, or USPS yourself.

Packages stay in this browser’s `localStorage`. Each card shows the nickname (or the tracking number), the carrier, the status “Not checked yet”, and a link to that carrier’s public tracking page. Nothing is sent to carrier APIs, and statuses are never invented. Remove a card to delete it. If the list is empty, the page says no packages are saved yet and notes that UPS account shipping history since Sep 26, 2026 was empty.
