# Homepage reframe: learning and impact orgs (PLAN, not executed)

Source: Counterparts insight call with Tom Moore and Michael Narea, 2026-11-11 (Granola: https://notes.granola.ai/t/ea7625e9-b520-4686-a299-c1e6dc357365).
Status: **proposal**. `/` is unchanged. Nothing here is a logged decision yet; D-HQ-011 (the "3 ROI-positive AI agents" homepage) is still the current truth.

What exists on branch `learning-impact-offer`:

| Path | What it is |
|---|---|
| `/new-home` (`new-home.html`) | Prototype of the next homepage. `noindex`, not linked, not in the sitemap. Has a "prototype" ribbon. |
| `/ai-workflows` (`ai-workflows.html`) | The current homepage, moved to its own page so it can be sent directly. Canonical and og:url point to itself. `/` still serves the same content until cutover. |
| this file | The plan. |

---

## 1. The reframe in one paragraph

Stop looking for an ICP and create one. Lead with an uncomfortable truth David is perfectly placed to call out: **for a decade, learning has tracked numbers that prove nothing** (enrollments, completions, minutes, smile sheets, cost per learner), and those numbers deliver no impact and earn no referrals. Turn it into an opportunity: if none of the numbers make sense, build a new system. The offer raises the stakes from "3 workflows" to **"10x the impact of your learning organization by replacing your learning stack with an AI-native one, designed with you."** It is explicitly **done with you** (player-coach), it takes the **whole** learning and IT budget, and we only sell the whole thing (no pilots).

## 2. Sequencing (Tom's order, which I'd keep)

1. **Pick the uncomfortable truth.** Draft: "For a decade, learning has tracked numbers that prove nothing." (Spicier variant for live conversations: "bullshit numbers that deliver no impact and generate no referrals.")
2. **Write the offer as a document, not a website.** One page, Drive. Tom's point is real: the website is not the bottleneck. The prototype here is a thinking tool and a share link for Vedansh, not a reason to delay the doc.
3. **Run 8 to 10 uncomfortable-truth interviews** (people who left Chegg, Coursera, Udemy, Udacity, 2U, ETS-type orgs; Shruti at Counterparts). Use their language to sharpen the page.
4. **Then cut over `/`** using the checklist in section 6.

## 3. New homepage architecture (as built in the prototype)

Built on the existing `lxd.css` components plus a small page-specific style block. Order follows the same desire-minus-confusion logic as `docs/gtm-page-plan.md`.

| # | Section | Job | Notes |
|---|---|---|---|
| 0 | Nav | Truth, Offer, Player-coach, Why us, Writing, Book a call | **No "Other offerings" menu.** Those pages stay live and get sent directly. |
| 1 | Hero | Who it's for + the stakes | Eyebrow "For learning and impact organizations". H1 "10x the impact of your learning organization. Built with you." Right panel shows A (legacy LMS, vendor sprawl, completion rates) to B (one AI-native system, team building on it, outcomes funders believe). |
| 2 | The uncomfortable truth (dark band) | Name the enemy | The numbers, not the people. No company names on the page (see open question 4). |
| 3 | "Swap the numbers" (interactive) | Make the truth personal | Six flip cards: Enrollments to who can now do the job; Completion to skills demonstrated; Minutes to time to first outcome; Smile sheet to referrals at six months; Cost per learner to cost per outcome; Courses published to learning that adapts. Ends with "Can you report the back side today?" |
| 4 | The offer | Raise the stakes | Weeks 1 to 2 honest baseline; days 1 to 90 first AI workflows live; months 4 to 9 replace the stack; month 12+ prove it. Then "What goes / What you get". |
| 5 | Player-coach (**hidden** 2026-11-11 to streamline; markup kept in a comment) | The differentiator Tom said was missing | We play (Vedansh, build) / We coach (David) / You own it. Fit list (for / not for) and the rule: "We only take on whole transformations." |
| 6 | Why us | Credibility in learning, not banking | David's learning background, 100 School x BCG capability stats, learning-org logos, impact funders (Gates, Walton, MSDF, Reach, Owl), Max's quote. Enterprise bank cases removed. |
| 7 | Uncomfortable truth interviews (**hidden** until interviews are live on Substack and LinkedIn; markup kept in a comment) | The marketing engine | Invites people sick of the numbers to a 30-min conversation. Three interview prompts. This is the lead source Tom described. |
| 8 | Team | "Your player-coaches" | David as coach, Vedansh as player. |
| 9 | Final CTA | "Leave the vanity numbers at the door." | No other-offerings chips. |

What was dropped from the current homepage: the "3 ROI-positive agents" hero, the AI capability loop, the `/check` teaser, the enterprise bank case cards, the three logo marquees, and the Other offerings menu and chips. All still live on `/ai-workflows`.

## 4. Who it's for (the created ICP)

- Learning and impact organizations, roughly 20 to 200 people (Tom's anchor: ~50 people, ~$5M in revenue or donations).
- Mission runs on learning: workforce and career training, bootcamps, professional and executive education (MBA programs), nonprofits that teach, non-product learning companies.
- Still on a legacy LMS, print, or bootcamp-in-a-box. Outcome goals not moving, or funders asking for more than completions.
- An optimist leader. Not finance or biotech for now (risk-transfer buyers, slow trust, done-for-you only).
- Budget anchor (Tom): $200K to $300K a year from orgs with ~$500K for learning tools, IT and training.

## 5. Open questions for David and Vedansh

1. **Is "10x impact" defensible?** We need one story that shows a big multiple on an outcome, not a completion rate. If not yet, soften to "Multiply the impact..." until we have it.
2. **Timeline honesty.** Page says 90 days to first workflows and ~12 months to a full replacement. Vedansh framed the build as 12 to 24 months. Pick the promise we can keep.
3. **How spicy?** Page uses "numbers that prove nothing" and "vanity numbers". The "bullshit numbers" line works in conversations and maybe LinkedIn, probably not the homepage.
4. **Naming the fallen platforms** (Chegg, Coursera, Udemy, Udacity, Duolingo, ETS). Strong for interviews and posts; a Legal/Risk call for the homepage. Prototype keeps them off.
5. **Price on page?** D-HQ-010 kept price off B2B. Recommend the same here; qualify on the call.
6. **David's bio facts.** Confirm the "helped scale developer training across Africa" line and the exact years.
7. **What happens to `/check`?** It's an AI-maturity check for any org. Options: keep it in the footer only, or build a "Learning impact check" that scores the six flip-card pairs. The second fits the new story better.
8. **Proof gap.** Most strong proof is enterprise (JPM, Target, PNC) or GTM (100 School). We need one learning-org case where outcomes moved. Candidate interview targets double as case studies.

## 6. Cutover checklist (when we say go)

- [ ] Offer document written and reviewed (Drive), interviews started.
- [ ] Copy `new-home.html` over `index.html`; remove the prototype ribbon and `noindex`; restore GTM snippet, canonical, OG/Twitter tags, JSON-LD (new Service: "AI-native learning transformation, done with you").
- [ ] Archive the old homepage to `archive/index-YYYY-MM-DD.html` (same pattern as before).
- [ ] Add `/ai-workflows` to `sitemap.xml`; keep `/b2b`, `/product`, `/gtm`, `/education` live but unlinked from `/`.
- [ ] Update `llms.txt`, `check.md`, `/agents` copy so agents describe the new offer.
- [ ] New OG image (the truth line on navy).
- [ ] Rename `data-cta` events from `v2-*` to final names and check GTM triggers.
- [ ] Log the decision in HQ `DECISIONS.md` (new D-HQ entry, `Replaces: D-HQ-011` for homepage positioning) and update Now.
- [ ] Mobile and dark-band contrast check; Lighthouse pass.
