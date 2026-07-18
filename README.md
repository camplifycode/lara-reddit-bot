# Lara — Golf Daze Reddit bot

`u/lara_golfdaze` is the openly disclosed Reddit account of Golf Daze,
an Australian golf simulator business and authorised Full Swing partner
for ANZ.

## What it does
- Operates and moderates our community subreddit, r/FullSwingSimulatorAustralia:
  twice-weekly original posts (build guides, buying guides, community
  discussion prompts).
- Occasionally answers questions in related golf-simulator subreddits
  where genuine expertise helps (launch monitors, home sim room specs,
  Australian pricing/import questions).

## How it behaves
- Fully disclosed: the profile states the Golf Daze affiliation.
- Low volume: hard-capped at a handful of write actions per day, with a
  minimum 20-minute gap between any two writes.
- Respects subreddit rules; communities whose rules prohibit vendor
  participation are excluded automatically.
- Uses the Reddit Data API via OAuth well within free-tier rate limits.

## Implementation
Scheduled jobs (Vercel cron) → Reddit Data API (OAuth script app).
Drafting/relevance decisions are made with Anthropic's Claude, with every
action logged and human-reviewed. The production codebase is private as
it contains business logic; this repo documents the bot's behaviour.

## Contact
justin@golfdaze.co
