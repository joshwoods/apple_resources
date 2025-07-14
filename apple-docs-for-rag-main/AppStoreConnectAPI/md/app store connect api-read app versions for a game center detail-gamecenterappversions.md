

- App Store Connect API
-  Read app versions for a Game Center detail 

Web Service Endpoint

# Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/gameCenterAppVersions
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

`filter[enabled]`

`[string]`

`include`

`[string]`

Possible Values: `compatibilityVersions, appStoreVersion`

`limit`

`integer`

Maximum: `200`

`limit[compatibilityVersions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAppVersionsResponse

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
https://api.appstoreconnect.apple.com/v1/gameCenterDetails/83b895ff-7bfe-5056-1208-ffd0d6a74e46/gameCenterAppVersions?limit=5
```

```
{
  “data” : [ {
    “type” : “gameCenterAppVersions”,
    “id” : “1d9b87fb-80c4-44eb-a114-a51aeebd82fc”,
    “attributes” : {
      “enabled” : false
    },
    “relationships” : {
      “compatibilityVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/1d9b87fb-80c4-44eb-a114-a51aeebd82fc/relationships/compatibilityVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/1d9b87fb-80c4-44eb-a114-a51aeebd82fc/compatibilityVersions”
        }
      },
      “appStoreVersion” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/1d9b87fb-80c4-44eb-a114-a51aeebd82fc/relationships/appStoreVersion”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/1d9b87fb-80c4-44eb-a114-a51aeebd82fc/appStoreVersion”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/1d9b87fb-80c4-44eb-a114-a51aeebd82fc”
    }
  }, {
    “type” : “gameCenterAppVersions”,
    “id” : “6ee80093-de91-9073-a043-4e7dcd28ae7b”,
    “attributes” : {
      “enabled” : true
    },
    “relationships” : {
      “compatibilityVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/6ee80093-de91-9073-a043-4e7dcd28ae7b/relationships/compatibilityVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/6ee80093-de91-9073-a043-4e7dcd28ae7b/compatibilityVersions”
        }
      },
      “appStoreVersion” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/6ee80093-de91-9073-a043-4e7dcd28ae7b/relationships/appStoreVersion”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/6ee80093-de91-9073-a043-4e7dcd28ae7b/appStoreVersion”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/6ee80093-de91-9073-a043-4e7dcd28ae7b”
    }
  }, {
    “type” : “gameCenterAppVersions”,
    “id” : “7bb8ca27-b622-43e1-a838-15b18dc58421”,
    “attributes” : {
      “enabled” : true
    },
    “relationships” : {
      “compatibilityVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/7bb8ca27-b622-43e1-a838-15b18dc58421/relationships/compatibilityVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/7bb8ca27-b622-43e1-a838-15b18dc58421/compatibilityVersions”
        }
      },
      “appStoreVersion” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/7bb8ca27-b622-43e1-a838-15b18dc58421/relationships/appStoreVersion”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/7bb8ca27-b622-43e1-a838-15b18dc58421/appStoreVersion”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/7bb8ca27-b622-43e1-a838-15b18dc58421”
    }
  }, {
    “type” : “gameCenterAppVersions”,
    “id” : “97c63a59-3dee-a1b3-6bec-5f0a2245c445”,
    “attributes” : {
      “enabled” : true
    },
    “relationships” : {
      “compatibilityVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/97c63a59-3dee-a1b3-6bec-5f0a2245c445/relationships/compatibilityVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/97c63a59-3dee-a1b3-6bec-5f0a2245c445/compatibilityVersions”
        }
      },
      “appStoreVersion” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/97c63a59-3dee-a1b3-6bec-5f0a2245c445/relationships/appStoreVersion”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/97c63a59-3dee-a1b3-6bec-5f0a2245c445/appStoreVersion”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/97c63a59-3dee-a1b3-6bec-5f0a2245c445”
    }
  }, {
    “type” : “gameCenterAppVersions”,
    “id” : “a3d76fe2-5baf-e9e7-198f-dcec974711eb”,
    “attributes” : {
      “enabled” : true
    },
    “relationships” : {
      “compatibilityVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/a3d76fe2-5baf-e9e7-198f-dcec974711eb/relationships/compatibilityVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/a3d76fe2-5baf-e9e7-198f-dcec974711eb/compatibilityVersions”
        }
      },
      “appStoreVersion” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/a3d76fe2-5baf-e9e7-198f-dcec974711eb/relationships/appStoreVersion”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/a3d76fe2-5baf-e9e7-198f-dcec974711eb/appStoreVersion”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/a3d76fe2-5baf-e9e7-198f-dcec974711eb”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/83b895ff-7bfe-5056-1208-ffd0d6a74e46/gameCenterAppVersions?limit=5”,
    “next” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/83b895ff-7bfe-5056-1208-ffd0d6a74e46/gameCenterAppVersions?cursor=ODExNDMwNzYw.Wc8eXw&limit=5”
  },
  “meta” : {
    “paging” : {
      “total” : 14,
      “limit” : 5
    }
  }
}
```

## See Also

### Reading Game Center app versions

Read information for a specific app version

Read the Game Center enablement state and related app version information.

Read the App Store version for an app version

Read the app store version and related information for an app version.

Read compatibility version information

Get compatibility version information for a specific app version.

Read compatible app versions

List all compatible verisons for an app version.

