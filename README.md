# Phishing Simulation Summary Report

A practical PowerShell tool that turns Microsoft Defender phishing simulation CSV exports into a single-page, interactive HTML summary for management reporting.

## What this project provides

- One-command HTML report generation
- KPI summary for sent, opened, deleted, forwarded, replied, clicked, reported, and compromised users
- User lists by action with search, sorting, and copy support
- Local/offline output (single HTML file)
- Resilient parsing for imperfect CSV exports

## Requirements

- Windows PowerShell 5.1+ or PowerShell 7+
- No external dependencies required

## Quick start

Run with the included fictional sample:

```powershell
.\Generate-PhishingSummary.ps1 -CsvPath ".\fictional-phishing-simulation.csv" -OutHtmlPath ".\Phishing-Summary.html" -OpenReport
```

Run with your own Defender export:

```powershell
.\Generate-PhishingSummary.ps1 -CsvPath "C:\path\to\your-export.csv" -OutHtmlPath ".\Phishing-Summary.html" -OpenReport
```

## Project structure

- Generate-PhishingSummary.ps1: main report generator script
- fictional-phishing-simulation.csv: fictional demo input file
- LICENSE: MIT license
- README.md: project documentation

## Sample data notice

The sample CSV contains fictional names and emails created only for demonstration.

## License

MIT
