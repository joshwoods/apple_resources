

- App Store Connect API
-  Read the leaderboards in a leaderboard set 

Web Service Endpoint

# Read the leaderboards in a leaderboard set

List all leaderboards in a leaderboard set.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Reading leaderboard sets

Read leaderboard set information

Read information about a specific leaderboard set.

List leaderboard information for a leaderboard set

Read the leadboards that belong to a learderboard set.

List leaderboard sets in a group leaderboard set

List information about leaderboards and leaderboard sets in a group leaderboard set.

List all localizations for a leaderboard set

Get a list of localized metadata for a leaderboard set.

Read the group leaderboard set in a leaderboard set

List all the group leaderboard sets in a leaderboard set.

List releases for a leaderboard set

Read the state of releases for a leaderboard set and related information.

