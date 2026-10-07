# RTD logger data

Daily backups written automatically by the RTD logger server. One CSV per device per day:
`data/<device_id>/<year>/<YYYY-MM-DD>.csv`.

- The day in the file name is the calendar day in Asia/Kolkata; `timestamp_utc` inside is UTC.
- Columns: `ch1`..`ch8` in degrees Celsius, two decimals, empty when a sensor reported a fault.
- A file is rewritten if readings from that day arrive late (a logger that was offline catching up).
