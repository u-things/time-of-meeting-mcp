# Time of Meeting

Remote MCP server: https://timeofmeeting.com/mcp

Time of Meeting finds a fair meeting time across cities. Pass plain city names such as Bern or Zurich. An IANA time zone such as Europe/Zurich is also accepted. Work hours are 9:00–17:00 local. Saturday and Sunday are weekends. A city's public holiday down-ranks that slot. Date tools count calendar days, working days, week numbers, and ages, and they find the next weekday, the business-hour overlap on one date, and the next clock change.

Tools:

- `find_best_meeting_time` — propose up to three fair meeting times for two to eight cities.
- `business_hours_overlap` — work-hour overlap for two to eight cities on one date.
- `convert_time` — convert a local time in one city into other cities' time zones.
- `current_time_in_cities` — current local time and work-hour status for each city.
- `search_cities` — find cities by name, with id, IANA time zone, and country.
- `create_meeting_link` — a Time of Meeting planner link, with optional paste-ready text, an .ics file, a Google Calendar link, or a QR code.
- `get_holidays` — public holidays for a country, region, or city.
- `get_dst_changes` / `dst_check` — when a city's clocks change, and whether a planned local time is skipped or happens twice.
- `days_between`, `working_days_between`, `add_days`, `add_business_days` — calendar-day and business-day or bank-day counts and offsets.
- `next_occurrence` — the next first, second, third, fourth, fifth, or last weekday of a month.
- `week_number` — ISO week and US week for one date.
- `age_duration` — age or duration as calendar years, months, and days.
- `submit_feedback` — send feedback to the Time of Meeting team. Describe the problem, not the user, and leave out personal details.

About 60 requests per minute and 2000 per day for each IP address. There is no login.
