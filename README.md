# Assignment 3: Collaborating in Github

A collaborative R Markdown analysis hosted on Github of text messaging data across two groups and two timepoint. 
Colloaborators: Harsha Helsing and Manya Gupta 
Responsibilities: 
1. Github Repo Creation and ReadMe: Harsha 
2. vis 1: Manya
3. vis 2: Harsha 
4. Summary Stats and Desctiption: Manya

## Data Description

Amount of total text messages a person typed were captured for participants at two different time points for participants categorized into two groups. The data is found in the file `TextMessages.csv`.

- 50 participants across 2 groups (25 per group)
- Columns: Group, Baseline, Six_months, Participant
- Wide format with one row per participant

## Repository Structure

- `Assignment3.Rmd` — Main analysis file
- `Assignment3.pdf` — Knitted PDF output
- `TextMessages.csv` — Source data
- `.gitignore` — Excludes R proj files

## Analysis Overview

### Visualization 1: Faceted Boxplots (PR #3 - Manya)
Faceted boxplots comparing text message distributions by Group and Timepoint using `geom_boxplot` and `facet_wrap(~Group)`, color-coded by Timepoint with the Set2 palette.

### Visualization 2: Faceted Bar Charts (PR #1 - Harsha)
Two faceted bar charts showing mean text counts with 95% CI error bars and mean labels:
- Vis 2a: Group on x-axis, faceted by Timepoint
- Vis 2b: Timepoint on x-axis, faceted by Group

### Summary Statistics (PR #2)
Grouped summary table of text message counts (mean, SD, median, min, max, IQR) by Group and Timepoint, generated using `dplyr` and displayed with `kable`.

## Key Findings

- Both groups had similar baseline text message counts (~65 messages)
- Group 1 showed a larger decrease at six months (to ~53) with greater variability
- Group 2 showed a much smaller decrease (~65 to ~62) with consistent messaging patterns

## Branch and PR Workflow

Each team member worked on a separate branch and submitted a pull request:
- `Visualization_1` → PR #3
- `feature_branch_vis_2` → PR #1
- `summary_stats` → PR #2

## Packages Used

readxl, Hmisc, pastecs, tidyverse, knitr, car
