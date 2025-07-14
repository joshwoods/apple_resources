

- App Store Connect API
- Game Center
-  Game Center details 

API Collection

# Game Center details

Manage enablement, achievement, leaderboard, and localization details for your apps.

## Overview

Game Center details is the top-level endpoint for Game Center information for your apps. Use this resource to:

- Enable Game Center for an app.

- Read information about specific types of Game Center data, including achievements, leaderboards, and localizations.

To enable Game Center, begin by calling Enable Game Center for an app. Then you can create and configure achievements, leaderboards, leaderboard sets, and more.

## Topics

### Reading Game Center details

Read the state of Game Center for an app

Get Game Center detail information for an app.

Read Game Center details

Read a specific Game Center detail and related information.

Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

Read the groups in a Game Center detail

Get a list of groups in a Game Center detail.

### Creating and editing Game Center details

Enable Game Center for an app

Create a Game Center detail for an app.

Modify a Game Center detail for an app

Edit challenge state, default leaderboards, and groups.

Modify the associated leaderboard sets for a Game Center detail

Edit the associated leaderboard sets for a Game Center detail.

Modify the associated leaderboards for a Game Center detail

Edit the associated leaderboards for a Game Center detail.

### Reading and editing Game Center detail achievements

List all achievements

List all achievement information for a Game Center detail.

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

List achievements

List the achievements for a Game center detail.

Modify associated achievements

Modify the achievements for a Game center detail.

### Reading and editing Game Center detail leaderboards

Read leaderboard releases

List all leaderboard releases for a Game Center detail.

Read leaderboard information

Get all leaderboards and related information for a Game Center detail.

List leaderboards

​List all leaderboards for a Game Center detail.

### Reading and editing leaderboard sets in a Game Center detail

Read leaderboard set information

Get all leaderboard sets and related information for a Game Center detail.

List leaderboard sets

List all leaderboards for a Game Center detail.

Read leaderboard set release information

List all leaderboard set releases for a Game Center detail.

### Objects

object GameCenterDetail

The data structure that represents a Game Center detail resource.

object GameCenterDetailCreateRequest

The request body you use to create a Game Center detail.

object GameCenterDetailGameCenterAchievementsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and an achievement.

object GameCenterDetailGameCenterAchievementsLinkagesResponse

A response that confirms a relationship between a Game Center detail and an achievement.

object GameCenterDetailGameCenterLeaderboardSetsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and a leaderboard set.

object GameCenterDetailGameCenterLeaderboardSetsLinkagesResponse

A response that confirms a relationship between a Game Center detail and leaderboard set.

object GameCenterDetailGameCenterLeaderboardsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and a leaderboard.

object GameCenterDetailGameCenterLeaderboardsLinkagesResponse

A response that confirms a relationship between a Game Center detail and a leaderboard.

object GameCenterDetailResponse

A response that contains a single Game Center detail resource.

object GameCenterDetailUpdateRequest

The request body you use to update a Game Center detail.

object GameCenterDetailsResponse

A response that contains a list of Game Center detail resources.

## See Also

### Details and groups

Game Center groups

Manage groups between your apps.

