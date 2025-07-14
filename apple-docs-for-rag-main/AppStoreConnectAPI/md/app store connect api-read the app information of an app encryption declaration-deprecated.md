

- App Store Connect API
-  Read the App Information of an App Encryption Declaration Deprecated

Web Service Endpoint

# Read the App Information of an App Encryption Declaration

Get the app information from a specific app encryption declaration.

App Store Connect API 1.0+

Deprecated

Use Read an App’s Encryption Declarations to update the relationship to an app encryption declaration instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/{id}/app
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List App Encryption Declarations response.

## Query Parameters

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

AppWithoutIncludesResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/69ab60b8-2f7a-91d4-e053-5b8c7c110c82/app
```

```
{
  "data" : {
    "type" : "apps",
    "id" : "6446671329",
    "attributes" : {
      "name" : "Your Next Cortado",
      "bundleId" : "com.bdt.ync",
      "sku" : "YNC",
      "primaryLocale" : "en-US",
      "isOrEverWasMadeForKids" : false,
      "subscriptionStatusUrl" : null,
      "subscriptionStatusUrlVersion" : null,
      "subscriptionStatusUrlForSandbox" : null,
      "subscriptionStatusUrlVersionForSandbox" : null,
      "availableInNewTerritories" : true,
      "contentRightsDeclaration" : "DOES_NOT_USE_THIRD_PARTY_CONTENT"
    },
    "relationships" : {
      "ciProduct" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/ciProduct",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/ciProduct"
        }
      },
      "betaTesters" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/betaTesters"
        }
      },
      "betaGroups" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/betaGroups",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/betaGroups"
        }
      },
      "appStoreVersions" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appStoreVersions",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appStoreVersions"
        }
      },
      "preReleaseVersions" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/preReleaseVersions",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/preReleaseVersions"
        }
      },
      "betaAppLocalizations" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/betaAppLocalizations",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/betaAppLocalizations"
        }
      },
      "builds" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/builds",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/builds"
        }
      },
      "betaLicenseAgreement" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/betaLicenseAgreement",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/betaLicenseAgreement"
        }
      },
      "betaAppReviewDetail" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/betaAppReviewDetail",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/betaAppReviewDetail"
        }
      },
      "appInfos" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appInfos",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appInfos"
        }
      },
      "appClips" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appClips",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appClips"
        }
      },
      "appPricePoints" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appPricePoints",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appPricePoints"
        }
      },
      "pricePoints" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/pricePoints",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/pricePoints"
        }
      },
      "endUserLicenseAgreement" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/endUserLicenseAgreement",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/endUserLicenseAgreement"
        }
      },
      "preOrder" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/preOrder",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/preOrder"
        }
      },
      "prices" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/prices",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/prices"
        }
      },
      "appPriceSchedule" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appPriceSchedule",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appPriceSchedule"
        }
      },
      "availableTerritories" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/availableTerritories",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/availableTerritories"
        }
      },
      "appAvailability" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appAvailability",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appAvailability"
        }
      },
      "inAppPurchases" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/inAppPurchases",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/inAppPurchases"
        }
      },
      "subscriptionGroups" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/subscriptionGroups",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/subscriptionGroups"
        }
      },
      "gameCenterEnabledVersions" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/gameCenterEnabledVersions",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/gameCenterEnabledVersions"
        }
      },
      "perfPowerMetrics" : {
        "links" : {
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/perfPowerMetrics"
        }
      },
      "appCustomProductPages" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appCustomProductPages",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appCustomProductPages"
        }
      },
      "inAppPurchasesV2" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/inAppPurchasesV2",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/inAppPurchasesV2"
        }
      },
      "promotedPurchases" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/promotedPurchases",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/promotedPurchases"
        }
      },
      "appEvents" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/appEvents",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/appEvents"
        }
      },
      "reviewSubmissions" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/reviewSubmissions",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/reviewSubmissions"
        }
      },
      "subscriptionGracePeriod" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/subscriptionGracePeriod",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/subscriptionGracePeriod"
        }
      },
      "customerReviews" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/relationships/customerReviews",
          "related" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329/customerReviews"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/apps/6446671329"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/6c2ddd3b-6d5e-4535-95f9-ece2c72c3848/app"
  }
}

```

## See Also

### Getting App Encryption Declarations

List App Encryption Declarations

Find and list all available app encryption declarations.

Read App Encryption Declaration Information

Get information about a specific app encryption declaration.

Read a specific App Encryption Declaration Document

Get detailed information about a specified App Encryption Declaration document.

Read the Declaration Document for an App Encryption Declaration

Read the associate document for a specific App Encryption Declaration.

