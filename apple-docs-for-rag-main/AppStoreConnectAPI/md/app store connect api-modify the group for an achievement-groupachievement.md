

- App Store Connect API
-  Modify the group for an achievement 

Web Service Endpoint

# Modify the group for an achievement

Modify the achievement group for a specific achievement.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/{id}/relationships/groupAchievement
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List all achievements response.

## HTTP Body

GameCenterAchievementGroupAchievementLinkageRequest

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

### Creating, modifying, and deleting achievements

Create an achievement

Add an achievement to a Game Center detail.

Modify an achievement

Modify properties for a specific achievement.

Delete an achievement

Delete a specific achievement.

