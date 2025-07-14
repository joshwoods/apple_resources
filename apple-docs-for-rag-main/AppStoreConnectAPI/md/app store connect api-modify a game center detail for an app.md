

- App Store Connect API
-  Modify a Game Center detail for an app 

Web Service Endpoint

# Modify a Game Center detail for an app

Edit challenge state, default leaderboards, and groups.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterDetailUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterDetailResponse

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

Modify the associated leaderboard sets for a Game Center detail

Edit the associated leaderboard sets for a Game Center detail.

Modify the associated leaderboards for a Game Center detail

Edit the associated leaderboards for a Game Center detail.

