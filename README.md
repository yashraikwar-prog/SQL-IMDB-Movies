🎬 IMDb Movies SQL Database Project

This project involves designing and managing a MySQL database to store and analyze IMDb-style movie data. The schema is built with relevant fields like Movie Name, Rating, Genre, Year, and Duration.

### 🗂️ Table Created:
**Table Name:** `movies`

| Column Name   | Data Type | Description                       |
|---------------|-----------|-----------------------------------|
| MovieID       | int       | Unique movie identifier           |
| Movie_Name    | text      | Name of the movie                 |
| Rating        | double    | Average user rating               |
| Votes         | int       | Number of votes received          |
| Meta_Score    | int       | Metacritic score (if available)   |
| Genre         | text      | Movie genres                      |
| PG_Rating     | text      | Parental rating (e.g., PG-13)     |
| Year          | int       | Year of release                   |
| Duration      | text      | Duration of movie (e.g., 2h 10m)  |

### ⚙️ Technologies Used:
- MySQL Workbench
- SQL (DDL commands)
- Local MySQL Server

### 🔧 How to Use:
1. Open the `create_imdb_movies_table.sql` file in MySQL Workbench.
2. Execute the script to create the `movies` table.
3. Insert data and run SQL queries to explore movie insights.

### ✅ Sample Queries You Can Try:
```sql
-- Top 5 highest rated movies
SELECT Movie_Name, Rating FROM movies ORDER BY Rating DESC LIMIT 5;

-- Movies released after 2015
SELECT * FROM movies WHERE Year > 2015;

-- Total number of votes by genre
SELECT Genre, SUM(Votes) AS Total_Votes FROM movies GROUP BY Genre;
````

### 📌 Project Status:

✔️ Table created
⏳ Data population and analysis queries – Coming soon!





