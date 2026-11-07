# Lunar Cycle Reset Protocol for Leaf-Insect Projects

Use this protocol at each New Moon / Full Moon checkpoint, or whenever a project cycle is intentionally archived and restarted.

## Purpose

The cycle reset prevents long-running chat drift and keeps the project portable between discussions. It creates a clean archive of the completed cycle, a concise status file, and a fresh append-only log for the next cycle.

## Trigger

Run the protocol when a lunar checkpoint reminder fires, or when the keeper manually declares a checkpoint.

Recommended reminder text:

> ⚠️ Generate the enclosure log summary snapshot and status summary for the Full Moon/New Moon checkpoint.

## Outputs to generate

### 1. Full log extract

Create an Excel workbook containing the complete chronological log for the cycle being closed.

Recommended columns:

- Date
- Temperature average / min / max
- Humidity average / min / max
- External weather context
- Interventions / husbandry
- Observations
- Confidence / notes

Rules:

- Use the previous archive filename/date range as the authoritative boundary marker.
- Do not restart arbitrarily from recent days.
- Include missing-data rows explicitly when daily stats were not provided.
- If values are estimated from screenshots rather than exact exports, mark them as approximate.

### 2. Status update text file

Create a short English text file, usually a few paragraphs, summarizing:

- date range covered
- current enclosure setup
- main environmental findings
- husbandry changes
- population status
- unresolved questions or watch points
- next-cycle priorities

The status file should be readable as a handoff note in a new conversation.

### 3. Individuals status file

Export the current Individual Progression Table as a separate file.

This file should be changed only when one of these triggers occurs:

- confirmed molt
- new naming
- significant stage estimate change
- abnormal or suspect behavior
- new individual introduced
- individual death or removal

Routine environmental observations belong in the chronological log, not in the individuals file unless they change an individual’s status.

### 4. New cycle seed log

Start the next log with one single seed entry. After this, future days are appended without modifying previous entries.

The seed entry should include:

- cycle start date
- previous archive boundary
- current population summary
- current enclosure/husbandry baseline
- immediate watch points

## Append-only rule for the new cycle

Once the new cycle begins:

- add new dates as they arrive
- do not rewrite prior entries silently
- corrections should be added as correction notes
- flag missing daily stats proactively
- keep observations and interpretations distinct

## Data quality rules

When interpreting graphs or screenshots:

- verify the date shown on each screenshot
- confirm temperature and humidity screenshots refer to the same day
- distinguish enclosure data from outside weather data
- note when a graph is probably app-smoothed rather than raw continuous data
- do not infer causal effects before the actual event time

For example, if garden misting starts at 08:00, any causal enclosure response to misting can only start at or after 08:00. Apparent pre-08:00 curve movement should be treated as smoothing/interpolation or an unrelated trend.

## Recommended file names

Use consistent names so future cycles can find the boundary:

- `Project_full_log_extract_YYYYMMDD-YYYYMMDD.xlsx`
- `Project_status_update_New_Moon_YYYYMMDD.txt`
- `Project_status_update_Full_Moon_YYYYMMDD.txt`
- `Project_individuals_status_New_Moon_YYYYMMDD.md`
- `Project_individuals_status_Full_Moon_YYYYMMDD.md`
- `Project_next_cycle_seed_YYYYMMDD.md`

## For letiranti eggs or other projects

For egg projects, adapt the individuals file into an egg-batch status file. Suggested columns:

- Batch / container
- Species
- Egg count
- Expected morph/color if relevant
- Date received / laid if known
- Incubation substrate
- Temperature / humidity baseline
- Hatch events
- Failures / suspect eggs
- Notes and confidence

The same cycle reset structure applies: archive the completed log, export current batch status, write a status handoff, then start the next append-only log with a single seed entry.
