

- App Store Connect API
-  Delete a leaderboard release 

Web Service Endpoint

# Delete a leaderboard release

Delete a new leaderboard release.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardReleases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## See Also

### Managing leaderboard releases

List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

Read leaderboard release information

Read the state of a specific leaderboard release.

Create a leaderboard release

Add a new leaderboard release.

