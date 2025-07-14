

- App Store Connect API
- Game Center
-  Game Center player achievements 

API Collection

# Game Center player achievements

Manage Game Center achievements by player for your apps.

### Overview

This endpoint is different than most in App Store Connect API, this’s used to create or modify a player’s achievement in your app. Any and all data you send through this endpoint overwrites existing data for the player.

## Topics

### Creating Game Center player achievements

POST /v1/gameCenterPlayerAchievementSubmissions

Add a new entry for a player’s score for a Game Center achievement.

### Objects

object GameCenterPlayerAchievementSubmission

object GameCenterPlayerAchievementSubmissionCreateRequest

The request body you use to create an Game Center player achievement.

object GameCenterPlayerAchievementSubmissionResponse

A response that contains a single Game Center player achievement resource.

## See Also

### Achievements

Game Center achievements

Manage achievements for your apps.

Game Center achievements localizations

Manage localizations for your achievements.

Game Center achievements images

Manage images for your Game Center achievements.

Game Center achievement releases

Manage releases for your Game Center achievements.

