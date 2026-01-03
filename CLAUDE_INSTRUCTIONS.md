# VAFFL Season Report - Instructions for Claude

## Overview
This document contains instructions for generating the annual VAFFL fantasy football season report from Yahoo Fantasy Football screenshots.

## Input Data
- Screenshots of weekly matchup results from Yahoo Fantasy Football
- File naming convention: `week1.png`, `week2.png`, ... `week14.png`
- Each screenshot shows 5 matchups per week (10 teams total)

## Teams in League (as of 2025)
1. CCR
2. Saquon deez nutz
3. Who Flung Puka
4. CMC
5. Rockets
6. Gamehendge Comets
7. Angry Dragon
8. Velvet Evolver
9. Trailer Parkansas
10. Steel 'er Face

*Note: Team names may change year to year - extract from screenshots*

## Data to Extract from Each Screenshot
For each weekly matchup:
- Team name (left side)
- Team score (left side - bold number is final score)
- Team name (right side)
- Team score (right side - bold number is final score)

## Calculations Required

### 1. Season Totals
- Sum all 14 weekly scores for each team
- Sort teams by total points (highest to lowest)

### 2. Weekly Highlights
For each week, identify:
- **Highest score** (Gold/1st place)
- **Second highest score** (Silver/2nd place)
- **Lowest score** (Tomato/last place)

### 3. Medal Count
Count for each team:
- Total weekly golds (highest scores)
- Total weekly silvers (2nd highest scores)
- Total weekly tomatoes (lowest scores)

## Report Format

### Main Table
- Rows: Teams sorted by total points (highest first)
- Columns: W1, W2, W3... W14, TOTAL
- Highlighting:
  - Gold background for weekly highest
  - Silver background for weekly 2nd highest
  - Red/tomato background for weekly lowest

### Summary Section
Include:
- Most Weekly Golds (Highest): Team name and which weeks
- Most Weekly Silvers (2nd Highest): Team name(s) and count
- Most Weekly Tomatoes (Lowest): Team name and which weeks
- Highest Single Week: Team, week number, score
- Lowest Single Week: Team, week number, score
- Any ties worth noting

### Medal Count Table
- Sort by gold count (descending)
- Columns: Team, Gold, Silver, Tomato

## Output Files
1. `[YEAR]_VAFFL_Season_Report.html` - Formatted HTML report that can be opened in browser and printed/screenshot
2. Update this instructions file if process changes

## Emoji Key (for markdown/text output)
- 🥇 = Weekly highest (Gold)
- 🥈 = Weekly 2nd highest (Silver)
- 🍅 = Weekly lowest (Tomato)

## Tips
- Double-check arithmetic! Verify totals against Yahoo's official season totals if available
- Watch for ties in weekly scores
- Regular season is typically 14 weeks (may vary)
- The bold score in screenshots is the final score; smaller number below is projected score

## Verification
Always ask user to verify calculated totals against Yahoo's official totals to catch any arithmetic errors.
