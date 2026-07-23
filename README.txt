SOLVE ENERGY — WEBSITE PACKAGE
================================

WHAT'S IN HERE
--------------
index.html                  Homepage (calculator, how it works, services, process, proof, FAQ, quote)
contact.html                Contact form + direct contact details
support-ticket.html         Support ticket submission form
refunds-policy.html         Draft refunds policy (see note below)
complaints-handling.html    Draft complaints handling policy (see note below)

Energy Comparison, New Energy Tech, and Consumer Code pages have been
removed from navigation per request. Not included in this package.

HOW TO DEPLOY
-------------
This is a static site — no build step, no server-side code, no dependencies to install.

1. Keep all files in this folder together, in the same directory, on whatever
   you deploy with. The pages link to each other using relative paths
   (e.g. "contact.html"), so they'll break if separated.
2. Drag this whole folder into any static host — Netlify, Vercel, Cloudflare
   Pages, GitHub Pages, or a plain web server. index.html is the entry point.
3. No environment variables, build commands, or config needed.

NAVIGATION
----------
Every page now has a "Support" dropdown in the header (matching the footer's
Support column) linking to Contact us, Submit a Ticket, Refunds Policy, and
Complaints Handling Policy — so all four are reachable from anywhere on the site.

BEFORE THIS GOES LIVE, PLEASE REVIEW
-------------------------------------
- refunds-policy.html and complaints-handling.html are DRAFT TEMPLATES,
  not legal advice. Each has a visible notice on the page saying so. Have
  a lawyer check them against your actual terms, licensing, and current
  Australian Consumer Law obligations before treating them as binding.
- contact.html has placeholder phone/email details
  (1300 000 000 / hello@solveenergy.com) — swap these for the real ones.
- The footer now includes an Aboriginal and Torres Strait Islander land
  acknowledgment with both flags. This is written in Solve Energy's own
  words (not copied from any other business) — please confirm the wording
  and the specific Traditional Owners named (if you want to name a specific
  Country/region) are accurate for wherever Solve Energy actually operates.
- The three forms (quote, contact, ticket) currently show a fake success
  message on submit — none of them are wired to a real backend/email yet.

DESIGN NOTES
------------
- Fonts load from Google Fonts (Sora, Manrope, JetBrains Mono) — requires
  an internet connection when the page loads.
- The homepage's page-by-page scroll effect and 3D animations are scoped
  to screens 900px and wider; narrower screens get a simpler normal scroll.
