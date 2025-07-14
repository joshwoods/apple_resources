

- App Store Connect API
-  Edit the relationship between a leaderboard and a group leaderboard 

Web Service Endpoint

# Edit the relationship between a leaderboard and a group leaderboard

Modify the group leadboard to which a leaderboard belongs.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the leaderboard resource ID from the Read leaderboard information response.

## HTTP Body

GameCenterLeaderboardGroupLeaderboardLinkageRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, modifying, and deleting leaderboards

Create a leaderboard

Add a new leaderboard to your app.

Edit a leaderboard

Modify the details of a leaderboard.

Delete a leaderboard

Delete a leaderboard from your app.

