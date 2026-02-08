# Daily Ship

One automated commit per day: the workflow creates that day’s log entry and updates streak stats.

## How it works

1. A [GitHub Action](../.github/workflows/daily-log.yml) runs once per day (05:00 UTC) or on demand via **Run workflow**.
2. It creates **today’s entry** in `entries/` if missing (e.g. `entries/2025-02-09.md`).
3. It recomputes **streak** and **total days** and updates [STREAK.md](STREAK.md).
4. It commits and pushes changes to `daily-log/`.

Edit any day’s file in `entries/` (Shipped / Learned / Note) whenever you like; the bot only ensures the day exists and the stats are up to date.

## Layout

| Path | Purpose |
|------|--------|
| `entries/` | One `YYYY-MM-DD.md` per day (Shipped / Learned / Note). |
| `STREAK.md` | Auto-updated streak and total days. |
| `scripts/update-daily.sh` | Creates today’s entry and writes STREAK.md. |
