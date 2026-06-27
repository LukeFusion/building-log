# June 2026

## 2026-06-27: Shipped ApplyTrue v4 to production
**Shipped.** Cut over a contract-first rebuild of my job-application agent to prod: a deterministic tier-based fit-scoring rubric with knockouts, an agent-loop apply flow, and a rich fit-analysis view. 283 tests, a 6-for-6 production smoke test, tagged release. Did the cutover as an attended session with a written rollback point instead of a blind deploy. Lesson that keeps proving itself: the plan and the restore tag are cheaper than the incident.

## 2026-06-26: Automated my whole job-application intake
**Shipped.** My `/job-app` workflow now goes from a pasted job description to a tailored resume, cover letter, QA pass, and interview prep, and it auto-creates the tracking folder and logs the row via a Google Apps Script webhook. Every drafted output passes through an independent review agent before it's "done." The review loop adds latency; for application quality it's worth it.

## 2026-06-23: Built a local landing page for a consulting offer
**Shipped.** Stood up a standalone San Diego landing page for my AI-consulting side (Build with Luke), matched to the brand system, responsive, with a scrape-safe booking flow and no exposed contact details. Constraint drove the design: "no displayed email or phone" forced a cleaner funnel than I'd have built otherwise.

## 2026-06-10: Built a Rover business as a system, not a side hustle
**Shipped.** Turned our dog-boarding into a real operation: a bookings tracker, a demand-signal funnel (so declines still teach me something), a pricing strategy with staged raises, and canned auto-replies. Net take is ~72% of the customer-facing price, and now I can see it. Treating a $20/night gig like a product surfaced pricing power I was leaving on the table.

## 2026-06-03: Rebuilt my entire file system around purpose, not type
**Decided.** Reorganized years of work into four buckets by *what the work is for* (the business, the job search, life systems, side apps) instead of by file type. Wrote a migration plan and an execution map first, backed everything up, then ran it. Folder structure is a product decision: the taxonomy is the interface I use every day.
