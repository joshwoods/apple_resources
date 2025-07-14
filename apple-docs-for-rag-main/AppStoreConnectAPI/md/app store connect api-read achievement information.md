

- App Store Connect API
-  Read achievement information 

Web Service Endpoint

# Read achievement information

Read information about a specific Game Center achievement.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the achievement resource ID from the List all achievements response.

## Query Parameters

`fields[gameCenterAchievementLocalizations]`

`[string]`

Possible Values: `locale, name, beforeEarnedDescription, afterEarnedDescription, gameCenterAchievement, gameCenterAchievementImage`

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`limit[localizations]`

`integer`

Maximum: `50`

`limit[releases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAchievementResponse

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
https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAchievements
```

```
{
  “data” : [ {
    “type” : “gameCenterAchievements”,
    “id” : “d3888910-d5fd-4737-b903-2f54356ce682”,
    “attributes” : {
      “referenceName” : “Ristretto”,
      “vendorIdentifier” : “RISTRETTO_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/d3888910-d5fd-4737-b903-2f54356ce682”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAchievements”
  },
  “meta” : {
    “paging” : {
      “total” : 1,
      “limit” : 50
    }
  }
}
```

## See Also

### Reading achievements

List all achievements

List all achievement information for a Game Center detail.

List all localizations for an achievement

Read information about the release for specific achievement.

Read release information for an achievement

Read the state of an achievement release and related information.

List associated group achievement information for an achievement

Read information about the group for specific achievement.

List group achievements for an achievement

List associated group achievements for a specific achievement.

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

