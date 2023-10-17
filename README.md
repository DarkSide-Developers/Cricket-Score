# @darkside-developers/cricket-details

![npm](https://img.shields.io/npm/v/@darkside-developers/cricket-details)
![npm](https://img.shields.io/npm/l/@darkside-developers/cricket-details)

A Node.js library for fetching cricket match details, live scores, match news, featured matches, upcoming matches, and recently concluded matches.

## Installation

```javascript
npm install @darkside-developers/cricket-details


const cricket = require('@darkside-developers/cricket-details');

// Get match details
const matchDetails = cricket.cricket.match_url();
console.log(matchDetails);

// Get live score
const liveScore = cricket.cricket.live_score('https://www.example.com/live-match');
console.log(liveScore);

// Get match news
const news = cricket.cricket.match_news();
console.log(news);

// Get featured matches
const featuredMatches = cricket.cricket.feature_match();
console.log(featuredMatches);

// Get upcoming matches
const upcomingMatches = cricket.cricket.upcoming_match();
console.log(upcomingMatches);

// Get recent matches
const recentMatches = cricket.cricket.recently_match();
console.log(recentMatches);
```

```javascript
const cricket = require('@darkside-developers/cricket-details');

const upcomingMatches = cricket.cricket.upcoming_match();
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
