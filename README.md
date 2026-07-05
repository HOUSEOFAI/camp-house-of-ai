# CAMP HOUSE OF AI™ — THE OPENING DAY RUNBOOK
*Everything is built. This page is the match. Work top to bottom; the Camp opens at the bottom.*

---

## THE ASSETS (what exists, where it lives)

| Asset | File | Status |
|---|---|---|
| The Hub (landing page + registry + live Keeper chat) | `camp-site-index.html` | Built, endpoint-ready |
| The Lodge (daily thread + Camper's Logbook) | `camp-site-lodge.html` | Built, endpoint-ready |
| The Keeper's full ops prompt + 15 interview questions | `society-operations-kit.md` | Ready to paste |
| Email sequence (bunk-ready welcome, day 2, porch question) | `society-operations-kit.md` | Ready to paste |
| Morning Letters № 001–030 | `morning-letters-002-030.md` (+ № 001 in ops kit) | Written |
| The Morning Letter Press (daily skill machine, № 031+) | `morning-letter-press.html` | Working |
| Launch social copy (carousel + 7 posts + 5 fresh posts) | `society-invitation-suite.md`, `five-fresh-posts.md` | Written |
| Camp Patch icons + flow map + camper journey | `camp-patch-collection.html`, `society-full-flow.html`, `new-camper-journey.html` | Built |

---

## THE WIRES (in order)

**☐ 1. Build two receiving endpoints in your system / Lovable.**
- `POST /camp-registry` — receives `{name, email, source:"camp-registry", signed_at}` → creates contact, tags "camper"
- `POST /lodge-logbook` — receives `{name, skill_no, win, source:"lodge-logbook", posted_at}` → stores win
(Both pages already send exactly this JSON. Nothing to reformat.)

**☐ 2. Paste the two endpoint URLs.**
- In `camp-site-index.html`: find `const REGISTRY_ENDPOINT = "";` → paste URL
- In `camp-site-lodge.html`: find `const LODGE_ENDPOINT = "";` → paste URL

**☐ 3. Put the two pages on the web.**
- Lovable: drop both files into your project (index + lodge), or
- Vercel: hand me a token and I deploy in one command
- Keep filenames `index.html` and `lodge.html` so the doors between them work.

**☐ 4. Load the welcome automation in your sender.**
- Trigger: new "camper" contact
- Instantly: Email 1 — *"Your bunk at Camp is ready 🛶"* (ops kit; insert your live Lodge URL and Skill № 001 link)
- Daily at sunrise: drip Letters № 001–030 in order

**☐ 5. Seat the Keeper for email/DM.**
- Paste her full prompt (ops kit) into your inbox AI or a Claude Project
- Answer her 15 interview questions once — refund thresholds, sign-off, escalation rules
- Set flags: refunds over $[X], chargebacks, legal, private-engagement bookings, <90% confidence → you
- Schedule the nightly **Lights-Out Report** to your inbox
- (The on-page Keeper chat in the hub already works with no wiring.)

**☐ 6. Set the daily ritual (90 seconds/morning).**
- Pull the Letter Press lever (or use the pre-written letter of the day)
- Copy as Daily Lodge Thread → post as the new thread
- Copy as Morning Letter → confirm the drip matches
- Copy as IG Caption → post

**☐ 7. Light the beacon.**
- Bio line + pinned comment (invitation suite)
- Day 1: the 10-slide carousel, pinned
- Days 2–8: the seven launch posts, then rotate the five fresh posts

---

## OPENING DAY ORDER OF CEREMONY
1. Endpoints live → 2. Pages live → 3. Test-sign the registry with your own email → 4. Confirm "bunk is ready" arrives within a minute → 5. Confirm the Lodge logbook win lands in your system → 6. Ring the Keeper's bell, ask her three hard questions → 7. Post the carousel. **The Camp is open.**

---

## THE ONLY TWO DOORS THAT NEED YOU
Everything above runs itself. You appear only for:
- **The VIP Day** — $7,000, one devoted day
- **Witch Camp & the Magnificent Beast™** — $12,000 rising to $15,000, seven days, Denmark, Maine

The Keeper flags every warm inquiry in the Lights-Out Report. You take the porch conversations. That's the whole job now.

*— the House*
