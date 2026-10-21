---
name: alphabot-collab-raffles
description: >-
  Create Alphabot (alphabot.app) collab raffles from a partner brief using your
  team's existing templates, and pull raffle winners into spreadsheets. Use when
  asked to set up GTD/FCFS collab raffles or export Alphabot winners.
---
# Alphabot collab raffles

Requires a browser tool already signed in to Alphabot as a manager of `<YOUR_TEAM>`.
Team names, `<teamId>`s, which template is GTD (holders) vs FCFS (public), and your
Alphabot profile name come from memory / the getting-started skill. If missing, ask once and save.

## Hard safety rules
- **Never** connect a wallet, pay, buy boosts, or create/edit/delete templates.
- **Never press Enter** inside a form field: Alphabot submits the form on Enter. Click elsewhere or Tab out.
- **Always** show a summary + screenshots and get an explicit human OK before saving
  (unless the human said "run it"/"save" for this exact batch).
- Never pick, re-roll or delete winners unless asked.
- If not signed in, stop and ask the human to sign in. Never type credentials.

## Create raffles
1. **Read the partner brief** (Google Docs: fetch `<doc-url>/export?format=txt`). Extract: project name,
   blurb, X accounts to follow, Like & RT post URL, Discord invite (if any), chain, notes, winner counts,
   and the winner-submission deadline.
2. **Name** each raffle `<PARTNER> X <YOUR_TEAM> GTD` or `<PARTNER> X <YOUR_TEAM> FCFS` (team in caps).
   - **GTD** = holders / community template, visibility *Community*.
   - **FCFS** = public template, visibility *Public*.
3. Open `https://www.alphabot.app/new?teamId=<teamId>`, reload, and confirm the right team is selected.
   Pick the template from the **Raffle template** dropdown. Turn Auto-save off while drafting if available.
4. **Fill per-raffle fields only**: name, Type = *Raffle* (templates often leave it blank), winner count,
   **project data source** (search for `<PARTNER>` so banner/avatar fill in), description = partner blurb + notes.
5. **Blockchain**: set the partner's chain if the brief names it; else keep the default and say so.
   - *Gotcha*: picking the Project data source can switch Blockchain (e.g. to Ethereum); after choosing
     the project, set the chain back to the correct one.
6. **Tasks**: keep the template's X follows and **add** the partner's follows. Like & RT = partner post with
   **Require: Both**. Add a Discord requirement only if the brief asks.
7. **Winner info**: turn on **Direct to contract**; change nothing else there. Leave bot settings as templated.
   Auto finalize / auto announce: leave as the template has them (optional; ask if unsure).
8. Everything else stays as the template has it. Do not edit the template itself.
9. **Review**: send the human a summary (name, team, GTD/FCFS, visibility, winners, chain, follows, Like&RT,
   data source) plus screenshots. Wait for OK.
10. **Save**: click **SAVE & VIEW** once. If the page stays on the form or the raffle shows as a draft,
    click SAVE & VIEW again and verify the public raffle page loads.
11. Report each link with team, GTD/FCFS, visibility, winners, chain. Do batches one raffle at a time.

## Pull winners
1. Only raffles **you created** (match your profile name) that have ended and finalized.
2. Click the **Entries** icon, or open `https://www.alphabot.app/entries/<slug>`. In Winners, choose
   Export → Download as CSV.
3. Build one spreadsheet per partner/team with separate **GTD** and **FCFS** tabs. Columns: Discord username,
   Discord ID, X handle, wallet. Also offer tab-separated text for pasting.
4. Remind the human of the partner's submission deadline.

## Optional: hourly auto-pull routine
If your agent supports scheduled tasks, run hourly: list your raffles that finalized since the last run,
export winners as above, append to the sheet, and notify the human. Never re-roll or submit anywhere.
