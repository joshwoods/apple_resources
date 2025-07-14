

- App Store Connect API
-  List all groups to which a leaderboard belongs 

Web Service Endpoint

# List all groups to which a leaderboard belongs 

List associated group leaderboards for a specific leaderboard.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the leaderboard resource ID from the Read leaderboard information response.

## Response Codes

` 200 ``OK`

GameCenterLeaderboardGroupLeaderboardLinkageResponse

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

### Reading leaderboards

Read leaderboard information

Read information about a specific leaderboard.

Read group information for a leaderboard

Read the group leadboard to which a leaderboard belongs.

List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

