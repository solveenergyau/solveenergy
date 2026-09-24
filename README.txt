SOLVE ENERGY 2.0
================
Static site. No build step. Every file goes in the repository root, beside
index.html. Design system: Outfit (headings) / Inter (body) / JetBrains Mono
(labels), Sora for the logo wordmark only; bubble-panel layout, amber-to-sky
accent, sticky nav with Support dropdown, dark mode toggle, shared footer.

FILES
-----
index.html                 Homepage
technical-details.html     How the system works + how it gets built (interactive)
contact.html               Contact form + direct details
support-ticket.html        Support ticket form
refunds-policy.html        Draft policy — not legally reviewed
complaints-handling.html   Draft policy — not legally reviewed
privacy-policy.html        Draft policy — not legally reviewed
favicon.ico                48px icon — required for the logo in Google results
favicon-32/180/512.png     Icons — must stay beside the HTML
logo-512.png               Logo referenced by Open Graph and Organization JSON-LD

DEPLOY (GitHub Pages)
---------------------
1. Upload all files above to the repository root, overwriting the old ones.
2. Do NOT delete the CNAME file already in the repo — it holds the custom
   domain. Uploading these files does not touch it.
3. Pages rebuilds in about a minute. Hard-refresh (Ctrl/Cmd + Shift + R).

AFTER DEPLOY — REQUIRED
-----------------------
1. FORMS: activated. All three forms post to
   https://formsubmit.co/ajax/94d9555e8237bbda86023f6892eb6fdc
   which delivers to info@solveenergy.com.au. Send a test through the live
   assessment form after deploying and confirm the email arrives.
2. SEARCH: verify solveenergy.com.au in Google Search Console and request
   indexing. The favicon and Organization JSON-LD only take effect after a
   re-crawl, which can take days.
3. PHONE: contact.html still shows the placeholder 1300 000 000.
4. POLICIES: the three policy pages are drafts and need legal review.

VERIFY AFTER DEPLOY
-------------------
- https://www.solveenergy.com.au/ loads with the new hero and nav
- "How it works" in the nav opens technical-details.html at the top
- Theme toggle switches to dark and survives a refresh
- Every Support dropdown link resolves (no 404s)
- The page does not scroll sideways on a phone
