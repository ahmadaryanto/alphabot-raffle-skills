---
name: alphabot-getting-started
description: >-
  First-run onboarding for the Alphabot raffle-manager skills: collect the
  user's Alphabot teams, team IDs and template names before creating raffles.
---
# Alphabot raffle manager: getting started

Explain: "I create Alphabot collab raffles from partner briefs and pull winner lists into spreadsheets."

Ask one at a time:
1. **Signed in?** Is Alphabot signed in in my browser? If not, hand the screen over so they sign in.
   Never type credentials. Tip: it's better to try with a **new email that is part of your Alphabot team**
   (manager role) rather than your main account.
2. **Teams**: which teams do you manage? Get each link `https://www.alphabot.app/team/<teamId>`.
3. **Templates**: for each team open `https://www.alphabot.app/new?teamId=<teamId>` read-only, list the
   templates in the Raffle template dropdown, and ask which is **GTD (holders/community)** and which is
   **FCFS (public)**. Never create or edit templates.
4. **Profile name**: your Alphabot profile name, so winners are pulled only from raffles you created.
5. **Approval mode**: always show a summary first (recommended), or save directly when you say "run it"?

Save answers to memory, e.g.:
```
<YOUR_TEAM>: teamId=<teamId>, GTD template="<TEMPLATE_A>", FCFS template="<TEMPLATE_B>"
profile=<PROFILE_NAME>, approval=summary-first
```
Offer a spreadsheet connector for winner sheets and the optional hourly winner-pull routine, then ask for the first partner brief.
