# @darkside-developers/cricket-details

[![npm](https://img.shields.io/npm/v/@darkside-developers/cricket-details)](https://www.npmjs.com/package/@darkside-developers/cricket-details)
[![npm](https://img.shields.io/npm/dt/@darkside-developers/cricket-details)](https://www.npmjs.com/package/@darkside-developers/cricket-details)
![npm](https://img.shields.io/npm/l/@darkside-developers/cricket-details)


A Node.js library for fetching cricket match details, live scores, match news, featured matches, upcoming matches, and recently concluded matches.

## Installation & Result

### Live Matches Urls
```javascript
// Get Live matches urls
const { cricket } = require('@darkside-developers/cricket-details');

const matchDetails = cricket.match_url();
console.log(matchDetails);
```
```javascript
[
  {
    "status": true,
    "creator": {
      "name": "DarkWinzo",
      "github": "@DarkWinzo"
    },
    "result": {
      "title": "Match 1",
      "link": "https://www.cricbuzz.com/match1"
    }
  },
  {
    "status": true,
    "creator": {
      "name": "DarkWinzo",
      "github": "@DarkWinzo"
    },
    "result": {
      "title": "Match 2",
      "link": "https://www.cricbuzz.com/match2"
    }
  },
  ...
]
```

### Recently Match Details
```javascript
```
```javascript
```

### Recently Match Details
```javascript
// Get Recently match details
const { cricket } = require('@darkside-developers/cricket-details');

const upcomingMatches = cricket.upcoming_match();
console.log(upcomingMatches);
```
```javascript
{
  "status": true,
  "creator": {
    "name": "DarkWinzo",
    "github": "@DarkWinzo"
  },
  "upcoming": {
    "series": "Upcoming Series",
    "match": [
      {
        "header": "Match Header 1",
        "team_a": "Team A",
        "team_b": "Team B",
        "status": "Upcoming",
        "link": "https://www.cricbuzz.com/upcoming-match1"
      },
      {
        "header": "Match Header 2",
        "team_a": "Team C",
        "team_b": "Team D",
        "status": "Upcoming",
        "link": "https://www.cricbuzz.com/upcoming-match2"
      },
      ...
    ]
  }
}
```
