

- App Store Connect API
-  Create a leaderboard set release 

Web Service Endpoint

# Create a leaderboard set release

Add a new leaderboard set release.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetReleases
```

## HTTP Body

GameCenterLeaderboardSetReleaseCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardSetReleaseResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing leaderboard set releases

Read leaderboard set release information

Get information about a leaderboard set release.

Delete a leaderboard set release

Delete a new leaderboard set release.

