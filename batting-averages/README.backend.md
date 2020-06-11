# Batting Averages Backend Exercise

Batting average is simple and a common way to measure batter’s performance.
Create an app that will ingest a raw CSV file with player statistics and
provide will provide player rankings based on their batting performance.

## Input

The application should take an input in form of a CSV file. The file will be
comma separated CSV with headers. The headers that interest you are: “playerID”,
“yearID”, “stint”, teamID”, “AB”, and “H”.

The application should also accept filter options:
- Year
- Team name
- Year and Team name

When filter are present, the output should include only players that match
the filter, sorted according to their batting average.


## Expected output

Batting Average is calculated as: BA = H/AB (Hits / At Bats).

If the player has more stints in the season, calculate batting average for the
whole season (across all stints), team names are comma separated in that case.
Format the batting average to 3 decimals.

You can write a standalone command line app, or you can write a web API along
with simple client.

The output should be like a following table:

```
+----------+--------+--------------+-----------------+
| playerID | yearId | Team name(s) | Batting Average |
+----------+--------+--------------+-----------------+
| ...                                                |
+----------------------------------------------------+
```


## CSV files

The input CSV file is `Batting.csv`. This file includes "teamID", use the
file `Teams.csv` to map "teamID" to a team's real name. You can process the
teams file and have the data ready in your app to map out "teamID" to team
names, it doesn't need to be uploaded from the user.


## Guidelines

* Use any of the major languages that can be run on OSX
* The app can be command line or provide an API over HTTP with command line
  client
* Do not fork this repo, create a clean one for a solution
* Feel free to ask for any clarification

