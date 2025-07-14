

- App Store Connect API
-  List leaderboard sets 

Web Service Endpoint

# List leaderboard sets

List all leaderboards for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/relationships/gameCenterLeaderboardSets
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

GameCenterDetailGameCenterLeaderboardSetsLinkagesResponse

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

### Reading and editing leaderboard sets in a Game Center detail

Read leaderboard set information

Get all leaderboard sets and related information for a Game Center detail.

Read leaderboard set release information

List all leaderboard set releases for a Game Center detail.

