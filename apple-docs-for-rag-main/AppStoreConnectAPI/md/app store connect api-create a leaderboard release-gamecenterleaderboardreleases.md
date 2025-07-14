

- App Store Connect API
-  Create a leaderboard release 

Web Service Endpoint

# Create a leaderboard release

Add a new leaderboard release.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardReleases
```

## HTTP Body

GameCenterLeaderboardReleaseCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardReleaseResponse

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

### Managing leaderboard releases

List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

Read leaderboard release information

Read the state of a specific leaderboard release.

Delete a leaderboard release

Delete a new leaderboard release.

