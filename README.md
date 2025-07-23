# NPS Data Parser & Calculator

A web-based tool for converting raw NPS survey data into structured results for Excel analysis.

## Overview

This tool processes Net Promoter Score survey data by parsing percentage breakdowns and calculating the number of respondents in each category (Detractors, Passives, Promoters). Results are formatted for direct copying into Excel spreadsheets.

## Features

- Parse raw NPS percentage data from survey outputs
- Automatic calculation of respondent counts by category
- One-click copying to Excel in tab-separated format
- Data validation and error checking
- Clean, professional interface

## Usage

1. Paste raw NPS data containing percentage breakdowns for scores 0-10
2. Enter the total number of survey respondents
3. Click "Calculate NPS" to process the data
4. Click the results table to copy values for Excel

## Input Format

The tool accepts data in the following format:

```
NPS érték megoszlása
0 1 2 3 4 5 6 7 8 9 10
0% 0% 0% 10% 0% 0% 0% 0% 40% 20% 30%
```

No formatting or cleanup is required - paste the data exactly as exported from your survey tool.

## Test Examples

**Example 1 (10 respondents):**
```
0% 0% 0% 10% 0% 0% 0% 0% 40% 20% 30%
```
Results: 1 Detractor, 4 Passives, 5 Promoters

**Example 2 (25 respondents):**
```
4% 0% 8% 12% 0% 4% 0% 8% 16% 24% 24%
```
Results: 7 Detractors, 6 Passives, 12 Promoters

## Categories

- **Detractors (0-6):** Respondents who scored 0-6
- **Passives (7-8):** Respondents who scored 7-8  
- **Promoters (9-10):** Respondents who scored 9-10

## Technical Requirements

- Modern web browser
- No installation required
- Works offline after initial load

## Deployment

The tool runs as a single HTML file and can be:
- Hosted on GitHub Pages
- Deployed to any web server
- Run locally by opening the HTML file in a browser

## File Structure

- `index.html` - Complete application (HTML, CSS, JavaScript)
- `README.md` - This documentation
