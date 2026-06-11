# Task: Create May 2026 Monthly Recap & Cost Optimization Presentation

## Goals
- Calculate exact/estimated savings for migrating away from Recall AI & AWS to Spleen + self-hosted systems.
- Create a new, modern HTML/CSS presentation in the presentations repository for the May 2026 Monthly Recap (addressing current endeavors, data pipeline, and reflections).
- Verify the presentation and commit/push changes.

## Plan
1. [x] Research spending details for Recall AI, AWS, Railway, Zoom, and Spleen from CSVs or documentation.
   - Evidence: Found Recall AI ($367.00/mo), Railway ($10.00/mo), and Zoom (12 seats Pro) in the master subscription CSV.
2. [x] Calculate the cost savings if we switch to the Spleen plan + self-hosted n8n/Autobot.
   - Evidence: Estimated monthly savings of ~$293 to ~$307/mo ($3.5K to $3.6K/yr) by replacing Recall AI ($367) + Railway ($10) with Spleen ($70 - $84 for 10-12 Zoom users) and hosting on the existing Hetzner VPS ($0 incremental).
3. [x] Create the new presentation file `ai-dev-may-recap-and-cost-optimization.html` (renamed to reflect the topic).
   - Evidence: Created file `work_account_mark-weassist-io/presentations/ai-dev-may-recap-and-cost-optimization.html`.
4. [x] Verify the presentation structure and contents.
   - Evidence: Verified via chrome-devtools browser page load, snapshot checks, console checks (0 errors), and successful slide navigation (evaluated `currentSlide` state change).
5. [ ] Commit and push changes to the `mark-dev` branch.
