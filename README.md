# What's On Tampa Bay

Monthly calendar of free workouts, run clubs, business meetups, game nights, arts and festivals across St. Pete, Tampa and Pinellas County.

Live at **https://whatsontampabay.com** (hosted on Cloudflare Pages; every commit to `main` publishes automatically).

## Editing events
Everything lives in `index.html`. Open it on GitHub, click the pencil icon, and search (Ctrl/Cmd+F) for:

- `const WEEKLY` – standing weekly meetups (`dow`: 0 = Sunday … 6 = Saturday)
- `const EVENTS` – dated events (`s` = start date `YYYY-MM-DD`, optional `e` = end date)

Useful fields: `t` title, `c` category, `time`, `loc` (end with the city), `rsvp` link, `free:true` or `price`, `area` (`"stpete"`, `"tampa"`, `"pinellas"`), `featured:true` for a ★ Featured listing.

Delete a line to remove an event. Commit, and the site updates in about a minute.

## Config (search in index.html)
- `SUBMIT_URL` – Tally event-submission form
- `FEATURE_URL` – Tally "Feature your event" form (blank = uses the submission form)
- `NEWSLETTER_URL` – Substack/beehiiv subscribe link (blank = box shows "Coming soon")
