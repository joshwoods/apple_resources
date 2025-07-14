

- App Store Connect API
- Game Center
-  Game Center leaderboards 

API Collection

# Game Center leaderboards

Create and manage leaderboards for your apps.

## Overview

Use leaderboards in your games so players can compare their scores against other players in the same game. When you configure leaderboards in App Store Connect, you specify details such as the scores to collect and how to order them.

For more information about how to use leaderboards in your app, see Configure leaderboards.

## Topics

### Reading leaderboards

Read leaderboard information

Read information about a specific leaderboard.

Read group information for a leaderboard

Read the group leadboard to which a leaderboard belongs.

List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

List all groups to which a leaderboard belongs 

List associated group leaderboards for a specific leaderboard.

List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

### Creating, modifying, and deleting leaderboards

Create a leaderboard

Add a new leaderboard to your app.

Edit a leaderboard

Modify the details of a leaderboard.

Edit the relationship between a leaderboard and a group leaderboard

Modify the group leadboard to which a leaderboard belongs.

Delete a leaderboard

Delete a leaderboard from your app.

### Objects

object GameCenterLeaderboardUpdateRequest

The request body you use to update a leaderboard.

object GameCenterLeaderboardsResponse

A response that contains multiple leaderboard resources.

object GameCenterLeaderboard

The data structure that represent a leaderboard resource.

object GameCenterLeaderboardCreateRequest

The request body you use to create a leaderboard.

object GameCenterLeaderboardResponse

A response that contains a single leaderboard image resource.

object GameCenterLeaderboardGroupLeaderboardLinkageRequest

The request body you use to attach an individual leaderbaord to a group leaderboard.

object GameCenterLeaderboardGroupLeaderboardLinkageResponse

A response confriming a relationship between a leaderboard and group leaderboard.

## See Also

### Leaderboards

Game Center leaderboard images

Read and manage image assets for Game Center leaderboards.

Game Center leaderboard releases

Read, create, and delete Game Center leaderboards releases.

Game Center leaderboard localizations

Manage localizations for Game Center leaderboards.

Game Center leaderboards scores

Create and modify Game Center leaderboards scores.

