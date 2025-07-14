

- App Store Connect API
-  Read leaderboard release information 

Web Service Endpoint

# Read leaderboard release information

Read the state of a specific leaderboard release.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardReleases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboard`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterLeaderboard`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardReleaseResponse

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

### Managing leaderboard releases

List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

Create a leaderboard release

Add a new leaderboard release.

Delete a leaderboard release

Delete a new leaderboard release.

