# What I didn't build, and why

A PM's judgment shows as much in what gets shelved as in what ships. Two real examples from the projects above.

## SpreadSense: paused the hosting migration mid-fix

**Situation:** SpreadSense's live demo went down — the Railway backend app had been deleted outside my control, and the Neon database access was gone with it. Not a code bug; an infrastructure loss.

**What I did:** Diagnosed the failure directly (confirmed via a direct request to the Railway URL, bypassing the frontend, that the app no longer existed), then looked for a path back to a working demo: restored a dormant Supabase project as a Postgres replacement, evaluated Render as a backend host, and prepared a one-command Render Blueprint (`render.yaml`) so the actual redeploy would be a single approval away.

**What I didn't do:** Finish the migration. Standing it back up meant creating a new paid-tier account, accepting its free-tier pause/deletion policy, and committing to ongoing account management — a cost and operational decision, not an engineering one. I flagged that explicitly and paused rather than silently spending money or creating a dependency on my own judgment of what tier to pick.

**Why this is the right call, not a stall:** the fix was technically ready to execute — pausing wasn't avoidance, it was recognizing that re-platforming a demo is a product-owner decision (is the live demo worth a recurring cost right now, versus the GitHub repo and README doing the job for a portfolio review) that shouldn't get made by default just because the engineering path was clear.

## CreditResolve: chose not to build a backend

**Situation:** I wanted to test whether a specific loan-bucket taxonomy (Classified / Non-Accrual / Principal Recovery & Active Charge-Offs / Suspects) and a responsibility-centre rollup would actually feel right to someone managing problem loans.

**What I did:** Built the full interaction model — sortable tables, drill-downs, comment history, CRUD — against mock data only, in days, and shipped it labeled honestly as a vibe-coded prototype.

**What I didn't do:** Build persistence, auth, or a multi-user assignment model behind the associate column, even though those are the obvious "next" features a real product needs.

**Why:** the question I was actually answering — is this taxonomy right — gets answered by clicking through the UI, not by the backend. Building real infrastructure first would have meant paying full engineering cost before knowing if the structure itself was worth keeping. Naming the gap explicitly (no backend, mock data, resets on refresh) in the README was itself the product decision: better to make one honest claim than an inflated one that gets caught later.
