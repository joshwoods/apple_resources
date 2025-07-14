

- App Store Connect API
-  Read Game Center achievement release information 

Web Service Endpoint

# Read Game Center achievement release information

Read the state of a specific achievement release.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the Game Center achievement release resource ID from the List achievement releases  response.

## Query Parameters

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterAchievement`

## Response Codes

` 200 ``OK`

GameCenterAchievementReleaseResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/b46850bc-ba02-3793-4ea7-36738b92440a
```

```
{
  “data” : {
    “type” : “gameCenterAchievementReleases”,
    “id” : “b46850bc-ba02-3793-4ea7-36738b92440a”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/b46850bc-ba02-3793-4ea7-36738b92440a”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/b46850bc-ba02-3793-4ea7-36738b92440a”
  }
}
```

## See Also

### Managing Game Center achievement releases

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

Read release information for an achievement

Read the state of an achievement release and related information.

Create a Game Center achievement release

Create a release for an achievement and a Game Center detail.

Delete a Game Center achievement release

Delete a release of an achievement or Game Center detail.

