

- App Store Connect API
-  Modify the associated leaderboard sets for a Game Center detail 

Web Service Endpoint

# Modify the associated leaderboard sets for a Game Center detail

Edit the associated leaderboard sets for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/relationships/gameCenterLeaderboardSets
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterDetailGameCenterLeaderboardSetsLinkagesRequest

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

### Creating and editing Game Center details

Enable Game Center for an app

Create a Game Center detail for an app.

Modify a Game Center detail for an app

Edit challenge state, default leaderboards, and groups.

Modify the associated leaderboards for a Game Center detail

Edit the associated leaderboards for a Game Center detail.

