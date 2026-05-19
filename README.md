# IPL Match Analytics

An end-to-end data analysis project on Indian Premier League (IPL) matches using ball-by-ball cricket data. This project explores how toss decisions, innings phases, wickets, and dot balls influence match outcomes in T20 cricket.

---

## Project Objective

The goal of this project was to analyze IPL match data and answer key cricket analytics questions such as:

- Does winning the toss actually help teams win matches?
- Which innings phase has the biggest impact on winning?
- How do wickets and dot balls affect match outcomes?
- Who were the top-performing batters and bowlers in recent IPL seasons?

---

## Dataset

- Source: Cricsheet IPL ball-by-ball dataset
- Format: JSON converted into CSV using Python
- Total Records: ~289,000+ deliveries
- Each row represents one ball bowled in an IPL match

### Key Features Used

- `match_id`
- `season`
- `toss_winner`
- `winner`
- `batting_team`
- `over`
- `runs_total`
- `wicket_kind`
- `batter`
- `bowler`

---

## Data Cleaning & Preprocessing

The following preprocessing steps were performed:

- Removed non-result matches (`tie`, `no result`)
- Removed super-over innings
- Standardized inconsistent team names
- Standardized season formatting
- Handled missing values in wicket-related columns
- Created match-level dataset for toss analysis

---

## Feature Engineering

Additional analytical features were created:

### Phase Segmentation
- Powerplay (0–5)
- Middle Overs (6–14)
- Death Overs (15–19)

### Other Features
- Toss win indicator
- Match winner indicator
- Dot-ball indicator
- Wicket indicator

---

## Key Analyses Performed

### 1. Toss Impact Analysis
Compared win percentages of:
- Toss Winners
- Toss Losers

### 2. Phase-wise Run Analysis
Compared average runs scored by:
- Winning Teams
- Losing Teams

across all innings phases.

### 3. Wicket Analysis
Analyzed average wickets lost per phase for:
- Winning Teams
- Losing Teams

### 4. Dot Ball Percentage Analysis
Compared dot-ball percentages between:
- Winning Teams
- Losing Teams

### 5. Top Player Analysis
Identified:
- Top 5 batters by runs
- Top 5 bowlers by wickets
(2021–2025 seasons)

---

## Key Findings

| Question | Finding |
|---|---|
| Does winning the toss help? | Only slightly — toss winners won 51.5% of matches |
| Most impactful phase | Middle overs (6–14) showed the biggest scoring gap |
| Wicket pattern | Losing teams lost more wickets, especially in death overs |
| Dot-ball impact | Losing teams played significantly more dot balls |
| Top batter (2021–2025) | Shubman Gill — 2,927 runs |
| Top bowler (2021–2025) | Harshal Patel — 104 wickets |

---

## Most Interesting Insight

> I expected the death overs to have the greatest impact on match outcomes, but the analysis revealed that the middle overs created the largest scoring gap between winning and losing teams.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Visualizations Included

- Toss win percentage comparison
- Phase-wise scoring analysis
- Wicket-loss analysis
- Dot-ball percentage analysis
- Top player tables

---

## Conclusion

The analysis revealed that winning the toss has only a minor impact on IPL match outcomes, whereas consistent batting performance across all innings phases — especially during the middle overs — plays a much more significant role in determining victory. Winning teams also maintained better momentum by losing fewer wickets and playing fewer dot balls throughout the innings. Additionally, players like Shubman Gill and Harshal Patel demonstrated exceptional consistency across recent IPL seasons.

---

## Author

Kushal Pandya  
AI/ML Enthusiast | Data Analytics | Machine Learning
