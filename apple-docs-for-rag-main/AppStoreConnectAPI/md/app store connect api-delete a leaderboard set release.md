

- App Store Connect API
-  Delete a leaderboard set release 

Web Service Endpoint

# Delete a leaderboard set release

Delete a new leaderboard set release.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetReleases/{id}
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

### Managing leaderboard set releases

Read leaderboard set release information

Get information about a leaderboard set release.

Create a leaderboard set release

Add a new leaderboard set release.

