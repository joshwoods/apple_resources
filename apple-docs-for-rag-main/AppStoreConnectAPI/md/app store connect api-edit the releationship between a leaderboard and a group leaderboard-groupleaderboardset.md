

- App Store Connect API
-  Edit the releationship between a leaderboard and a group leaderboard 

Web Service Endpoint

# Edit the releationship between a leaderboard and a group leaderboard

Modify the group leaderboards in a leaderboard set.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSets/{id}/relationships/groupLeaderboardSet
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest

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

### Creating, editing, and deleting leaderboard sets

Create a leaderboard set

Add a new leaderboard set to your app.

Create a relationship between a leaderboard and a leaderboard set

Add a leaderboard to a leaderboard set.

Edit a leaderboard set

Modify the metadata for a leaderboard set.

Modify the leaderboards in leaderboard set

Edit the positions of leaderboards in an existing leaderboard set.

Delete a leaderboard set

Delete a specifc leaderboard set.

Delete the relationship between a leaderboard and a leaderboard set

Remove a leaderboard from a leaderboard set.

