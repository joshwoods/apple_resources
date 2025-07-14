

- App Store Connect API
-  List leaderboards 

Web Service Endpoint

# List leaderboards

​List all leaderboards for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/relationships/gameCenterLeaderboards
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

GameCenterDetailGameCenterLeaderboardsLinkagesResponse

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

### Reading and editing Game Center detail leaderboards

Read leaderboard releases

List all leaderboard releases for a Game Center detail.

Read leaderboard information

Get all leaderboards and related information for a Game Center detail.

