# Netflix-Dashboard
1. Documentation of Client Requirements
Overview of the Business
The client is a media streaming analytics team that wants to use historical and almost real-time data to examine content performance across films and TV shows, much like Netflix.

2. Goals
The customer requires a dashboard in order to:
Keep track of all stuff, including TV series and films.
Examine the distribution of content by: Country and Genre, Ratings by Year
Determine the best performers: Actors, Directors, and Genres
Make it possible to filter between TV shows and films.
Give business users interactive exploring options.

3. Requirements for Data
Sources of Data:
CSV Files (Python-based web scraping)
Metadata about the content (title, genre, cast, nation, ratings)
Live Connection SQL Server
Current data on streaming and content performance
Functional Requirements
KPI Cards: Total Shows, Total Countries, Total Number of Directors, All Genres, Beginning and Ending Years
Type of Filters/Slicers: TV Show/Movie, Director, Genre, Release Year Range
Visualisations : Shows by Country (Map) , Shows by Release Year Trend , Shows by Type (TV vs. Film) , Rating by Genre , Shows Count by Genre , Detailed Table (List of Shows and Movies)
Navigating Pages: Home (summary), Shows Movies  Non-Functional Conditions
Quick performance using a variety of data sources
Safe access by RLS
Simple user interface
The ability to refresh CSV and SQL data

3. The Solution Offered
Integration of Data
CSV (Python-Scraped Web)
Power Query was used to clean
used for historical and static metadata
SQL Server (Live Connection) through standard gateway
used for updated or dynamic data
DirectQuery or live connection ,Integrated through data modelling linkages Data Model
Table of Facts TV series and films
Dimensions: Date, Director, Country, and Genre
Relationships created for dashboard design slicing and filtering

Page 1: Overview (Home)
KPI Cards (Genres, Directors, Countries, and Shows)
Visualisation of a map (by country)
Trend graph (year of release)
Analysis based on genre

Page 2: Displays
Comprehensive TV Show Table
Filters
Director's genre
Drill-down capability

Page 3: Films
A structure similar to that of shows
Concentrate on film-specific analysis
UI/UX Design
layout with a dark Netflix vibe
Unambiguous segmentation
Interactive cutters
Button-driven navigation

4. Distribution of Content Derived from Analysis and Insights
The majority of the content originates from North America, Europe and Asia came next.
Genre Perspectives
Leading Genres: Reality Television, Dramatic Action on TV
indicates that viewers favour content with a lot of entertainment.
Trend for the Year
Content increased sharply after 2000.
Growth peak after 2015
shows the period of the streaming boom
Analysis of Ratings :
Highly regarded genres: Drama in Reality TV , Ideal places to invest in content creation
Television vs. Film: TV series are the most popular.
Movies that are marginally lower yet still noteworthy
Country Insights
The US produces the most content. Next in line are UK, India, Canada

5. Issues Resolved
Handled data refresh vs. real-time balance
Combined multiple CSV + live SQL data
Developed a scalable model for data in the future
Enhanced performance in spite of mixed sources
Configured Gateway in power BI service for automated refreshes.
