# earnings-bot-trigger

Public scheduler that triggers the private `Earningstranscriptbot` repo every weekday morning.

## Setup (one time)

1. Create a GitHub PAT at https://github.com/settings/tokens
   - Classic token → check **repo** (full) and **workflow**
   - No expiry (or set 1 year and calendar-remind yourself)
2. In THIS public repo → Settings → Secrets → Actions → New secret
   - Name: `PAT_TOKEN`
   - Value: the token you just created
3. Enable Actions on this repo if not already enabled

That's it. The workflow runs every weekday at 12:30 UTC and dispatches the private bot.
