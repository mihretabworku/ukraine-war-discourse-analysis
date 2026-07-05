# Data Directory

This directory contains documentation for the datasets used in this research.

## Data Sources

- **Primary**: Telegram messages scraped from pro-Russian channels during defined event windows
- **Scope**: 18 major conflict events (Feb 2022 – Jan 2026)

## Privacy & Ethics

Raw message data is **not included** in this repository to respect:
- Telegram's Terms of Service
- User privacy considerations
- Research ethics guidelines

The analysis scripts in `src/` can be used with similarly structured CSV data.

## Data Schema

The pipeline outputs a CSV with the following columns:

| Column | Type | Description |
|--------|------|-------------|
| `event_code` | string | Event identifier (E01–E18) |
| `message_date` | datetime | Message timestamp |
| `channel` | string | Source channel name |
| `text` | string | Message content |
| `views` | int | View count |
| `forwards` | int | Forward count |
| `reactions` | int | Total reactions |
| `theme` | string | Classified thematic category |
| `category` | string | Broader category grouping |
