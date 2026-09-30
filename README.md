# MSS Sim: interactive walkthrough

**Live demo: https://zash3.github.io/mss-sim/**

A clickable, self-contained walkthrough of diagnosing a late nightly BI refresh on a Microsoft BI estate
(SQL Server Agent, SSISDB, SSMS, perfmon). It follows the "Late on Sundays" incident: read the ticket, find
the pattern in the job history, locate the slow layer in the SSIS catalog, query the maintenance log in an
SSMS-style window, confirm the mechanism in perfmon, name the root cause, and fix the schedule.

- One HTML file, no build step, no network requests: open `index.html` in any browser.
- Data is generated in the page from a fixed seed, so every visit sees the same estate.
- Keyboard friendly: F5 runs the query, Ctrl+K jumps to a step, Esc closes dialogs. Deep links like `#sql` open a step directly.
