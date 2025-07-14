

- App Store Connect API
-  Read leaderboard set release information 

Web Service Endpoint

# Read leaderboard set release information

Get information about a leaderboard set release.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetReleases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardSetReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboardSet`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterLeaderboardSet`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetReleaseResponse

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

### Managing leaderboard set releases

Create a leaderboard set release

Add a new leaderboard set release.

Delete a leaderboard set release

Delete a new leaderboard set release.

