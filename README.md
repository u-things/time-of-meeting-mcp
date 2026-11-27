# Time of Meeting for Gemini CLI

This extension adds the Time of Meeting MCP server to [Gemini CLI](https://github.com/google-gemini/gemini-cli). It holds config only, with no code. Gemini CLI connects to the remote server at `https://timeofmeeting.com/mcp` over streamable HTTP.

Time of Meeting finds a fair meeting time across two to eight cities, converts local times, and builds planner and calendar links. It also counts business days and bank days, with bank closing days kept separate from public holidays.

It has 16 read-only tools. They don’t change anything in your accounts or contact other services on your behalf. It’s free. You don’t need an account, a login or an API key.

## Install

You need Gemini CLI and git. Run this in your terminal, not inside a Gemini CLI session:

```sh
gemini extensions install https://github.com/u-things/time-of-meeting-mcp
```

Then start Gemini CLI, or restart it if it’s already open. To check that it worked, type `/extensions list` or `/mcp` in Gemini CLI. `/mcp` shows the server, whether it’s connected, and its tools.

## Update or remove

```sh
gemini extensions update time-of-meeting-mcp
gemini extensions uninstall time-of-meeting-mcp
```

Restart Gemini CLI after either one.

## What you can ask

- Find a fair time next week for a call between Copenhagen, New York, and Singapore.
- How many business days are there in Denmark between December 1, 2026 and January 8, 2027? Which public holidays fall in that span? Use bank days instead if banks must be open.
- US clocks change in March 2027. Does 2:30 AM on March 14, 2027 exist in New York? When do the clocks change there?

## What it can do

- Find up to three meeting times that work for everyone in two to eight cities, each with a score and reasons.
- Show where work hours overlap on a date.
- Convert one city’s local time into the time in other cities.
- Show the current local time and work-hour status in several cities.
- Look up a city’s time zone and country.
- List public holidays for a country, region, or city.
- Check when a city’s clocks change, and whether a planned time is skipped or happens twice.
- Count days, business days, or bank days between dates, add days or business days to a date, and get week numbers and ages.
- Make a link that opens the meeting in the Time of Meeting planner, with optional text to paste, a calendar file, an add-to-Google-Calendar link, or a QR code.

Business-day and bank-day coverage is 2026, 2027, and 2028. Bank days are available for US Federal Reserve holidays, Danmarks Nationalbank closing days, UK bank holidays, and TARGET2 euro closing days.

## Limits

Each IP address can make about 60 requests a minute and 2,000 a day. If you go over, the server answers “Rate limit exceeded” and says when to retry.

## Privacy and terms

Your assistant sends the server only what a tool needs, such as city names, dates, and times. The [privacy page](https://timeofmeeting.com/privacy) explains what we receive, what we keep, and what we count.

- Privacy: https://timeofmeeting.com/privacy
- Terms: https://timeofmeeting.com/terms
- Setup and docs: https://timeofmeeting.com/docs

## License

MIT. See [LICENSE](LICENSE).

## Contact

Questions? Email contact@u-things.com.
