

- App Store Connect API
- Game Center
-  Game Center leaderboards scores 

API Collection

# Game Center leaderboards scores

Create and modify Game Center leaderboards scores.

## Overview

This endpoint is different than most in App Store Connect API, with this you can create or modify a player’s leaderboard score in your app. Any and all data you send through this endpoint overwrites existing data for the player’s score.

Tip

These endpoint requires information from GameKit, specifically gamePlayerID.

## Topics

### Managing Game Center leaderboard scores

POST /v1/gameCenterLeaderboardEntrySubmissions

Add a new score for a player to a leaderboard.

### Objects

object GameCenterLeaderboardEntrySubmission

The data structure that represent an Game Center leaderboard entry submission resource.

object GameCenterLeaderboardEntrySubmissionCreateRequest

The request body you use to create an Game Center leaderboard entry submssion.

object GameCenterLeaderboardEntrySubmissionResponse

A response that contains a Game Center leaderboard entry submission.

## See Also

### Leaderboards

Game Center leaderboards

Create and manage leaderboards for your apps.

Game Center leaderboard images

Read and manage image assets for Game Center leaderboards.

Game Center leaderboard releases

Read, create, and delete Game Center leaderboards releases.

Game Center leaderboard localizations

Manage localizations for Game Center leaderboards.

