# July 2026

## 2026-07-21: Taught my automation to notice its own clock drifting
**Shipped.** My morning job runner had been firing hours off its intended time, and the reason nobody caught it is that three separate observers all wrote down the actual fire time and not one of them compared it to the scheduled one. Fixed it with a preflight that diffs the config file against what the system scheduler actually loaded, plus a 24-hour dead-man's switch on my monitoring system's own status email. One deliberate constraint: the drift check compares config to config and never looks at observed start time, so a legitimate catch-up run can't masquerade as a fault. Verified against a sandboxed copy with a 48-check harness, so no real jobs fired and no real mail went out.

## 2026-07-19: Put a real test gate in front of production
**Shipped.** Merged a Playwright end-to-end suite into ApplyTrue's main branch and wired it into CI, so every future pull request to production has to clear it before it can land. Small merge, seven files, test code only. Vercel deployed clean, GitHub Actions went green including the new e2e job, and I still smoke-tested all four public surfaces by hand before calling it done. Tests start protecting you at the moment they become a gate somebody has to pass through.

## 2026-07-06: Built an AI pipeline that talks me out of bad ideas
**Decided.** Ran two new app ideas (a weather-opportunity app and a habit tracker) through a "vet-idea" pipeline I built: it drafts a competitive brief, then routes the idea past three specialized agents (product, strategy, marketing) for an independent verdict. Both came back "shelve, validate first." The useful part isn't the yes, it's the fast, structured no. I baked a 5-screen passive-income filter into the pipeline so weak ideas fail early instead of eating a weekend.

## 2026-07-01: Shipped a story-map generator skill
**Shipped.** Built a command that turns any product's context into an interactive user-story-map (the Agile three-tier board: activities > tasks > stories-by-release) as a single drag-drop HTML file. Point it at a product, get a working board seeded from the real docs. Turned a recurring manual artifact into one command.
