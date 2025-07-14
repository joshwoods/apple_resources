

- App Store Connect API
-  Delete a Game Center achievement release 

Web Service Endpoint

# Delete a Game Center achievement release

Delete a release of an achievement or Game Center detail.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the Game Center achievement release resource ID from the List achievement releases  response.

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

### Managing Game Center achievement releases

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

Read release information for an achievement

Read the state of an achievement release and related information.

Read Game Center achievement release information

Read the state of a specific achievement release.

Create a Game Center achievement release

Create a release for an achievement and a Game Center detail.

