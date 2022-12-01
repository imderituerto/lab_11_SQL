# Football Matches - Tasks

Each of the questions/tasks below can be answered using a `SELECT` query. When you find a solution copy it into the code block under the question before pushing your solution to GitHub.

--Ed Hulbert: SELECT x WHERE x AND x OR x;

1) Find all the matches from 2017.

```sql
SELECT * FROM matches WHERE season ='2017';


```

2) Find all the matches featuring Barcelona.

```sql
SELECT * FROM matches WHERE hometeam ='Barcelona' OR awayteam ='Barcelona';


```

3) What are the names of the Scottish divisions included?

```sql
SELECT name FROM divisions WHERE country = 'Scotland';


```

4) Find the division code for the Bundesliga. Use that code to find out how many matches Freiburg have played in the Bundesliga since the data started being collected.

```sql
SELECT code FROM divisions where name = 'Bundesliga';
SELECT * FROM matches WHERE (hometeam = 'Freiburg' OR awayteam = 'Freiburg') AND division_code = 'D1';


```

5) Find the unique names of the teams which include the word "City" in their name (as entered in the database)

```sql
SELECT hometeam FROM matches WHERE hometeam LIKE '%City%' GROUP BY hometeam;


```

6) How many different teams have played in matches recorded in a French division?

```sql
<!-- Copy solution here -->


```

7) Have Huddersfield played Swansea in the period covered?

```sql
<!-- Copy solution here -->


```

8) How many draws were there in the Eredivisie between 2010 and 2015?

```sql
--Colin: MORE THAN ONE WAY TO DO THIS
<!-- Copy solution here -->


```

9) Select the matches played in the Premier League in order of total goals scored from highest to lowest. Where there is a tie the match with more home goals should come first.

```sql
<!-- Copy solution here -->


```

10) In which division and which season were the most goals scored?

```sql
<!-- Copy solution here -->


```

### Useful Resources

- [Filtering results](https://www.w3schools.com/sql/sql_where.asp)
- [Ordering results](https://www.w3schools.com/sql/sql_orderby.asp)
- [Grouping results](https://www.w3schools.com/sql/sql_groupby.asp)