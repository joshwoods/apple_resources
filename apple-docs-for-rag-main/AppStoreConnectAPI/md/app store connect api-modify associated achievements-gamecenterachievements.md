

- App Store Connect API
-  Modify associated achievements 

Web Service Endpoint

# Modify associated achievements

Modify the achievements for a Game center detail.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/relationships/gameCenterAchievements
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterDetailGameCenterAchievementsLinkagesRequest

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

### Reading and editing Game Center detail achievements

List all achievements

List all achievement information for a Game Center detail.

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

List achievements

List the achievements for a Game center detail.

