

- App Store Connect API
-  List all achievements 

Web Service Endpoint

# List all achievements

List all achievement information for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/gameCenterAchievements
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the Game Center detail resource ID from the Read the state of Game Center for an app response.

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

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`filter[archived]`

`[string]`

`filter[id]`

`[string]`

`filter[referenceName]`

`[string]`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`limit`

`integer`

Maximum: `200`

`limit[localizations]`

`integer`

Maximum: `50`

`limit[releases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAchievementsResponse

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
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAchievements
```

```
{
  “data” : [ {
    “type” : “gameCenterAchievements”,
    “id” : “304e0f56-63b2-492f-980e-bce6fafb8502”,
    “attributes” : {
      “referenceName” : “Perfectly Steamed Milk Texture”,
      “vendorIdentifier” : “PSMT_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : true,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502”
    }
  }, {
    “type” : “gameCenterAchievements”,
    “id” : “b5c383e5-c451-4cfe-9b31-9519c4106843”,
    “attributes” : {
      “referenceName” : “Fastest Service”,
      “vendorIdentifier” : “FS_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b5c383e5-c451-4cfe-9b31-9519c4106843”
    }
  }, {
    “type” : “gameCenterAchievements”,
    “id” : “b1392192-da63-4156-a39c-82f1278d465e”,
    “attributes” : {
      “referenceName” : “Cold Brew Timing”,
      “vendorIdentifier” : “CBT_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/b1392192-da63-4156-a39c-82f1278d465e”
    }
  }, {
    “type” : “gameCenterAchievements”,
    “id” : “ced67adc-b153-46f0-9d4c-3ee649a35267”,
    “attributes” : {
      “referenceName” : “Just Sweet Enough”,
      “vendorIdentifier” : “JSE_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/ced67adc-b153-46f0-9d4c-3ee649a35267”
    }
  }, {
    “type” : “gameCenterAchievements”,
    “id” : “10735ae0-55a7-4c3f-88f8-737a93fe0a36”,
    “attributes” : {
      “referenceName” : “Bean Blend”,
      “vendorIdentifier” : “BB_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/10735ae0-55a7-4c3f-88f8-737a93fe0a36”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAchievements?limit=5”
  },
  “meta” : {
    “paging” : {
      “total” : 5,
      “limit” : 5
    }
  }
}
```

## See Also

### Reading achievements

Read achievement information

Read information about a specific Game Center achievement.

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

