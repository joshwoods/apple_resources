

- App Store Connect API
- Game Center
-  Game Center leaderboard sets 

API Collection

# Game Center leaderboard sets

Manage Game Center leaderboard sets for your apps.

## Overview

Leaderboard sets organize several leaderboards into a single unit. For example, in a game that includes many levels, you might define a leaderboard set to organize the leaderboards for each level. A single app can have 100 leaderboard sets, and a set can have a maximum of 100 leaderboards. You must have at least one leaderboard for your app before you can create a leaderboard set. Once you add leaderboard sets to your app, all future leaderboards that you configure for the app must be included in a leaderboard set.

The process to start using leaderboard sets to organize your app’s leaderboards includes these steps:

- Create the first leaderboard set.

- Create additional leaderboard sets.

- Add new leaderboards directly into leaderboard sets.

For more information about how to use Leaderboard sets in your app, see Configure leaderboards sets.

## Topics

### Reading leaderboard sets

Read leaderboard set information

Read information about a specific leaderboard set.

List leaderboard information for a leaderboard set

Read the leadboards that belong to a learderboard set.

List leaderboard sets in a group leaderboard set

List information about leaderboards and leaderboard sets in a group leaderboard set.

List all localizations for a leaderboard set

Get a list of localized metadata for a leaderboard set.

Read the leaderboards in a leaderboard set

List all leaderboards in a leaderboard set.

Read the group leaderboard set in a leaderboard set

List all the group leaderboard sets in a leaderboard set.

List releases for a leaderboard set

Read the state of releases for a leaderboard set and related information.

### Creating, editing, and deleting leaderboard sets

Create a leaderboard set

Add a new leaderboard set to your app.

Create a relationship between a leaderboard and a leaderboard set

Add a leaderboard to a leaderboard set.

Edit a leaderboard set

Modify the metadata for a leaderboard set.

Modify the leaderboards in leaderboard set

Edit the positions of leaderboards in an existing leaderboard set.

Edit the releationship between a leaderboard and a group leaderboard

Modify the group leaderboards in a leaderboard set.

Delete a leaderboard set

Delete a specifc leaderboard set.

Delete the relationship between a leaderboard and a leaderboard set

Remove a leaderboard from a leaderboard set.

### Objects

object GameCenterLeaderboardSet

The data structure that represent a leaderboard set resource.

object GameCenterLeaderboardSetCreateRequest

The request body you use to create a leaderboard set.

object GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest

The request body you use to create a relationship between a leaderboard set and a leaderboard.

object GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse

A response that confirms a relationship between a leaderboard set and a leaderboard.

object GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest

The request body you use to create a relationship between a leaderboard set and a group leaderboard set.

object GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse

A response that confirms a relationship between a leaderboard set and a group leaderboard set.

object GameCenterLeaderboardSetResponse

A response that contains a single leaderboard set resource.

object GameCenterLeaderboardSetUpdateRequest

The request body you use to update a leaderboard set.

object GameCenterLeaderboardSetsResponse

A response that contains multiple leaderboard set resources.

## See Also

### Leaderboard sets

Game Center leaderboard set localizations

Manage localizations for your Game Center leaderboard sets.

Game Center leaderboard set images

Mangage image assets for your Game Center leaderboard sets.

Game Center leaderboard set releases

Manage a leaderboard set releases.

Game Center leaderboard set member localizations

Mangage Game Center leaderboard set member localizations.

