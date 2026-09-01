🏏 IPL Data Analysis Dashboard (2008–2025)

An interactive and comprehensive IPL Data Analysis Dashboard built using Microsoft Power BI, covering 18 seasons of Indian Premier League data from 2008 to 2025.

The project analyzes 1,169 IPL matches and provides season-wise, team-wise, and player-wise insights through interactive KPIs, DAX measures, dynamic slicers, team/player statistics, and professionally designed Power BI visuals.

📊 Dashboard Preview



Interactive Power BI dashboard covering IPL seasons from 2008 to 2025.

🎯 Project Objectives

Analyze IPL performance data from 2008 to 2025.

Clean and transform raw datasets using Power Query.

Build a structured relational data model in Power BI.

Create analytical measures using DAX.

Develop an interactive and professional Power BI dashboard.

Analyze team and player performance across seasons.

Identify important batting and bowling achievements.

Present complex cricket statistics through easy-to-understand visualizations.

Demonstrate practical Data Analyst / Business Intelligence skills.

📅 Dataset Information

Attribute

Details

Sport

Cricket

Tournament

Indian Premier League (IPL)

Seasons

2008–2025

Number of Seasons

18

Matches

1,169

Players

772

Match Data

Match-level IPL statistics

Ball-by-Ball Data

Delivery-level performance data

The project combines multiple datasets to create a relational Power BI data model.

🗂️ Dataset Structure

1. Match Dataset

ipl_matches_data_cleaned.csv

Contains match-level information such as:

Match ID

Season

Match Date

City

Venue

Teams

Toss Winner

Toss Decision

Match Winner

Win by Runs

Win by Wickets

Player of the Match

Match Stage

Match Result

2. Player Dataset

players-data-updated.csv

Contains player-related information including:

Player ID

Player Name

Full Name

Batting Style

Bowling Style

Player Image

The dataset contains 772 player records.

3. Team Dataset

teams_data.csv

Contains information related to IPL teams including:

Team ID

Team Name

Team Short Name

Team Logo/Image URL

4. Ball-by-Ball Dataset

The ball-by-ball dataset contains delivery-level information used for detailed player and performance analysis.

Important fields include:

Match ID

Batter

Bowler

Batter Runs

Extras

Wickets

Wicket Type

Delivery information

🔄 Data Preparation & Cleaning

The raw IPL data was prepared using Power Query before building the dashboard.

Major data preparation steps included:

Removing unnecessary columns

Handling missing values

Standardizing column names

Correcting data types

Cleaning date columns

Standardizing team names

Standardizing player names

Handling inconsistent date formats

Preparing image URL columns

Creating relationships between datasets

Validating match and season information

Creating cleaned versions of source tables

Power Query Techniques Used

Transform

Replace Values

Change Data Type

Custom Columns

Conditional Columns

Error handling

Text transformations

Date transformations

Data validation

🧩 Data Model

The project uses a relational data model inside Power BI.

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
        │ team information
        ▼
ipl_matches_data_cleaned

The match table provides season and match-level filtering, while the ball-by-ball table enables detailed delivery-level player analysis.

🧮 DAX & Calculations

DAX was extensively used to create dynamic KPIs and analytical measures.

Match Statistics

Total Matches

Total Teams

Total Venues

Matches Won

Matches Lost

Win Margins

Toss Impact

Batting Statistics

Total Runs

Total Fours

Total Sixes

Half-Centuries

Centuries

Highest Run Scorers

Top Run Scorer by Season

Bowling Statistics

Total Wickets

Top Wicket Takers

Purple Cap Holder

Bowling Performance

Season Statistics

Season Winner

Runner-up

Season-wise Team Performance

Season-wise Batting Performance

Season-wise Bowling Performance

📌 Key Dashboard KPIs

The dashboard dynamically displays important season-level KPIs such as:

💥 Total Sixes

🏏 Total Fours

🏟️ Total Matches

👥 Total Teams

5️⃣0️⃣ Half-Centuries

💯 Centuries

🏟️ Total Venues

All major KPIs respond dynamically to the selected IPL season.

🏆 Dashboard Features

🥇 Champion & Runner-Up

The dashboard dynamically identifies:

🏆 Season Champion

🥈 Runner-Up

Team Logos

When a season is selected, the Champion and Runner-Up automatically update.

🟠 Orange Cap Analysis

The Orange Cap section highlights the leading run scorer of the selected season.

It displays:

Player Name

Total Runs

Team

Player Image

🟣 Purple Cap Analysis

The Purple Cap section identifies the leading wicket-taker of the selected season.

It displays:

Player Name

Total Wickets

Team

Player Image

💥 Top Four Analysis

The dashboard identifies the player with the highest number of fours in the selected season.

Metrics include:

Player Name

Number of Fours

Team

Player Image

🚀 Top Six Analysis

The dashboard identifies the player with the highest number of sixes in the selected season.

Metrics include:

Player Name

Number of Sixes

Team

Player Image

📋 Points Table

The interactive Points Table provides season-wise team standings.

Metric

Description

Logo

Team Logo

Team Name

IPL Team

Pld

Matches Played

Won

Matches Won

Lost

Matches Lost

NR

No Result

Tie

Tied Matches

Total Points

Team Points

The table dynamically changes according to the selected season.

🎛️ Interactive Features

Season Slicer

Users can select any IPL season from:

2008 → 2025

All major visuals and KPIs update automatically.

Dynamic Visuals

The dashboard dynamically updates:

Champion

Runner-Up

Team Logos

Player Images

Orange Cap

Purple Cap

Top Fours

Top Sixes

Points Table

Season KPIs

🎨 Dashboard Design

The dashboard was designed with an IPL-inspired professional theme.

Design Elements

IPL branding

Team logos

Player images

KPI cards

Rounded cards

Consistent typography

Interactive slicers

Color-coded sections

Clean dashboard layout

Visual hierarchy

Dynamic image URLs

The objective was to make the dashboard both analytically useful and visually engaging.

🛠️ Tools & Technologies

Microsoft Power BI

Used for:

Dashboard development

Data modeling

Data visualization

Interactive filtering

KPI creation

Report design

Power Query

Used for:

Data cleaning

Data transformation

Data preparation

Error handling

Data type conversion

DAX

Used for:

Measures

Dynamic KPIs

Season calculations

Player statistics

Team statistics

Ranking calculations

Conditional calculations

Microsoft Excel / CSV

Used for:

Raw data storage

Initial data inspection

Data preparation

Git & GitHub

Used for:

Version control

Project documentation

Project sharing

Portfolio development

📊 Skills Demonstrated

This project demonstrates practical skills in:

Data Analysis

Data Cleaning

Data Transformation

Power BI

Power Query

DAX

Data Modeling

Relational Data Modeling

Data Visualization

KPI Development

Interactive Dashboard Design

Analytical Thinking

Business Intelligence

Data Storytelling

GitHub & Project Documentation

📁 Recommended Repository Structure

IPL-Data-Analysis/
│
├── 📁 data/
│   ├── ipl_matches_data_cleaned.csv
│   ├── ball_by_ball_data.csv
│   ├── players-data-updated.csv
│   └── teams_data.csv
│
├── 📁 artifacts/
│   └── dashboard_screenshot.png
│
├── 📁 PowerBI/
│   └── IPL_Data_Analysis.pbix
│
└── 📄 README.md

🔍 Example Analysis Questions

The dashboard can be used to answer questions such as:

Season Analysis

Who won the IPL in a particular season?

Who was the runner-up?

How many matches were played?

How many teams participated?

How many venues were used?

Batting Analysis

Who scored the most runs in a season?

Who hit the most sixes?

Who hit the most fours?

Who scored the most centuries?

Who scored the most half-centuries?

Bowling Analysis

Who took the most wickets?

Who won the Purple Cap?

Which teams had the strongest bowling performance?

Team Analysis

Which team won the most matches?

Which teams qualified for the playoffs?

How did a team's performance change across seasons?

Which teams accumulated the most points?

💡 Key Insights

The dashboard enables users to identify patterns and trends such as:

Season-wise changes in team performance

Top-performing batsmen

Leading wicket-takers

Batting milestones

Team points and standings

Impact of toss decisions

Match-winning performances

Venue-wise match distribution

Changes in IPL team participation

Individual player dominance across seasons

📈 Analytical Value

Although IPL is a sports domain, the project demonstrates concepts that are directly applicable to real-world business analytics.

The same workflow can be applied to:

Customer Analytics

Sales Analytics

Marketing Analytics

Financial Analytics

Product Analytics

Operations Analytics

Sports Analytics

The project demonstrates how raw transactional data can be transformed into an interactive analytical solution that supports data-driven decision making.

🔄 End-to-End Power BI Workflow

Raw IPL Data
      ↓
Data Cleaning
      ↓
Power Query Transformation
      ↓
Data Modeling
      ↓
Relationships
      ↓
DAX Measures
      ↓
KPI Development
      ↓
Interactive Visualizations
      ↓
Dashboard
      ↓
Data-Driven Insights

🚀 How to Use the Project

Step 1 — Clone the Repository

git clone https://github.com/aishwary-wasnik1905/IPL-Data-Analysis.git

Step 2 — Open the Power BI File

Open the .pbix file using Microsoft Power BI Desktop.

Step 3 — Load the Data

If required, update the data source paths to point to the CSV files in the repository.

Step 4 — Refresh the Dataset

In Power BI Desktop:

Home → Refresh

Step 5 — Explore the Dashboard

Use the Select IPL Season slicer to explore different seasons from 2008 to 2025.

📌 Important Notes

The project covers 18 IPL seasons from 2008 through 2025.

The match dataset contains 1,169 matches.

Player and team images are loaded through publicly hosted image URLs.

Image URLs may depend on third-party hosting and can change over time.

Dashboard calculations depend on the underlying dataset and data model.

🚀 Future Improvements

Add detailed Player Analysis page

Add Team Analysis page

Add Player vs Player comparison

Add Team vs Team comparison

Add venue analysis

Add toss impact analysis

Add batting strike-rate analysis

Add bowling economy analysis

Add interactive drill-through pages

Add advanced tooltip pages

Add season-to-season player comparison

Add additional IPL seasons as new data becomes available

📚 Learning Outcomes

Through this project, I strengthened my understanding of:

Working with real-world datasets

Data cleaning and transformation

Power Query

Data modeling

Relationships between tables

DAX measures

Filtering and aggregation

Dynamic calculations

KPI design

Power BI visualization

Dashboard UX/UI

Data storytelling

👨‍💻 Author

Aishwary Wasnik

B.Tech – Computer Science & Engineering
National Institute of Technology, Raipur

Aspiring Data Analyst / Business Intelligence Professional

GitHub

@aishwary-wasnik1905

⭐ Support

If you found this project useful or interesting:

⭐ Star this repository

🍴 Fork the repository

📢 Share it with others interested in Data Analytics and Power BI

📌 About This Project

IPL Data Analysis (2008–2025) is an end-to-end Power BI project analyzing 18 seasons of IPL data. The project combines Power Query, DAX, data modeling, interactive slicers, dynamic KPIs, player/team analysis, and professional dashboard design to transform raw cricket data into meaningful and interactive insights.

🏏 Project Highlights

18 Seasons • 1,169 Matches • 772 Players • Power BI • Power Query • DAX

Built with ❤️ using Microsoft Power BI
