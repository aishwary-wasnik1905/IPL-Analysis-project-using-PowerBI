# 🏏 IPL Data Analysis Dashboard (2008–2025)

An interactive and comprehensive **IPL Data Analysis Dashboard** built using **Microsoft Power BI**, covering **18 seasons of Indian Premier League data from 2008 to 2025**.

The project analyzes **1,169 IPL matches** and provides season-wise, team-wise, and player-wise insights through interactive KPIs, DAX measures, dynamic slicers, team/player statistics, and professionally designed Power BI visuals.

---

## 📊 Project Overview

The Indian Premier League (IPL) generates a large amount of match, player, team, and ball-by-ball data every season.

This project transforms raw IPL datasets into an **interactive analytical dashboard** that helps users explore:

- 🏆 Season Champions and Runners-up
- 🏏 Batting performance
- 🎯 Bowling performance
- 💥 Sixes and Fours
- 💯 Centuries and Half-Centuries
- 🟠 Orange Cap winners
- 🟣 Purple Cap winners
- 📋 Team Points Tables
- 🏟️ Venues and Matches
- 👥 Team and Player performance
- 📈 Season-wise trends
- 🔎 Interactive player and team analysis

The dashboard allows users to select an IPL season and dynamically explore the corresponding statistics.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Analyze IPL performance data from **2008 to 2025**.
2. Transform and clean raw datasets using **Power Query**.
3. Build a structured relational data model.
4. Create meaningful analytical measures using **DAX**.
5. Develop an interactive Power BI dashboard.
6. Analyze team and player performance across seasons.
7. Identify important batting and bowling achievements.
8. Present complex cricket statistics through easy-to-understand visualizations.
9. Apply professional dashboard design and data visualization principles.
10. Demonstrate practical **Data Analyst / Business Intelligence** skills.

---

# 📅 Dataset Information

### Coverage

| Attribute | Details |
|---|---|
| Sport | Cricket |
| Tournament | Indian Premier League (IPL) |
| Seasons | 2008–2025 |
| Number of Seasons | 18 |
| Matches | 1,169 |
| Players | 772 |
| Teams Dataset | 16 team records |
| Match Data | Match-level IPL statistics |
| Ball-by-Ball Data | Delivery-level performance data |

The project combines multiple datasets to create a relational Power BI data model.

---

# 🗂️ Dataset Structure

The project uses multiple datasets including:

### 1. Match Dataset

**`ipl_matches_data_cleaned.csv`**

Contains match-level information such as:

- Match ID
- Season
- Match Date
- City
- Venue
- Teams
- Toss Winner
- Toss Decision
- Match Winner
- Win by Runs
- Win by Wickets
- Player of the Match
- Match Stage
- Match Result

---

### 2. Player Dataset

**`players-data-updated.csv`**

Contains player-related information such as:

- Player ID
- Player Name
- Full Name
- Batting Style
- Bowling Style
- Fielding Position
- Player Image

The dataset contains **772 player records**.

---

### 3. Team Dataset

**`teams_data.csv`**

Contains information related to IPL teams including:

- Team ID
- Team Name
- Team Short Name
- Team Logo/Image URL

---

### 4. Ball-by-Ball Dataset

The ball-by-ball dataset contains delivery-level information used for detailed player and performance analysis.

Important fields include:

- Match ID
- Batter
- Bowler
- Batter Runs
- Extras
- Wickets
- Wicket Type
- Delivery information

This dataset is used to calculate player-level batting and bowling statistics.

---

# 🔄 Data Preparation & Cleaning

The raw IPL data was prepared using **Power Query** before building the dashboard.

Major data preparation steps included:

- Removing unnecessary columns
- Handling missing values
- Standardizing column names
- Correcting data types
- Cleaning date columns
- Standardizing team names
- Standardizing player names
- Handling inconsistent date formats
- Creating/cleaning match stages
- Preparing image URL columns
- Creating relationships between datasets
- Validating match and season information
- Creating cleaned versions of the source tables

### Power Query Techniques Used

- `Transform`
- `Replace Values`
- `Change Data Type`
- `Custom Columns`
- `Conditional Columns`
- Error handling
- Text transformations
- Date transformations
- Data validation

---

# 🧩 Data Model

The project uses a relational data model inside Power BI.

The main tables include:

```text
ipl_matches_data_cleaned
        │
        │ match_id
        ▼
ball_by_ball_data

players-data-updated
        │
        │ player information
        ▼
ball_by_ball_data

teams_data
        │
        │ team name
        ▼
ipl_matches_data_cleaned
