# Batting Average App

Batting average is simple and common way to measure batter’s performance. Create
an app that will ingest a raw CSV file with player statistics and presents
simple UI for ranking and filtering players based on their batting performance.


## Interface

The application should take an input in form of a CSV file. The file will be
comma separated CSV with headers. The headers that interest you are: “playerID”,
“yearID”, “stint”, teamID”, “AB”, and “H”.

Batting Average is calculated as: BA = H/AB (Hits / At Bats).

Once the file is loaded, the user will view table sorted by Batting Average:

```
+----------+--------+-----------+-----------------+
| playerID | yearId | Team name | Batting Average |
+----------+--------+-----------+-----------------+
| ...                                             |
+-------------------------------------------------+
```

The table should be filterable by:

* Player (use autocomplete select)
* Year (simple select)
* Team

When filter is selected, the table presents players that match the filter,
sorted according to their batting average.


## CSV files

The input CSV file is `Batting.csv`. This file includes "teamID", use the
file `Teams.csv` to map "teamID" to a team's real name. You can process the
teams file and have the data ready in your app to map out "teamID" to team
names, it doesn't need to be uploaded from the user.


## Guidelines

* Use any of the major languages that can be run on OSX
* The app can be client only or client-server split, up to you
* Do not fork this repo, create a clean one for a solution
