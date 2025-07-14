

- App Store Connect API
-  List All App Infos for an App 

Web Service Endpoint

# List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appInfos
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appInfos]`

`[string]`

Fields to return for included related types.

Possible Values: `appStoreState, state, appStoreAgeRating, australiaAgeRating, brazilAgeRating, brazilAgeRatingV2, franceAgeRating, koreaAgeRating, kidsAgeBand, app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[appInfoLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `locale, name, subtitle, privacyPolicyUrl, privacyChoicesUrl, privacyPolicyText, appInfo`

`fields[appCategories]`

`[string]`

Fields to return for included related types.

Possible Values: `platforms, subcategories, parent`

`fields[ageRatingDeclarations]`

`[string]`

Fields to return for included related types.

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

`limit[appInfoLocalizations]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppInfosResponse

`OK`

Request succeeded.

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

Use this endpoint to retrieve the derived app-level information for an app. If the app has both a “Ready for Sale” version and a version you’re preparing for release, it will have two app infos. One represents information about the app currently in the App Store, and the other represents the information that takes effect when you release the next version. Use the `appStoreState` attribute to differentiate them.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/1462965264/appInfos
```

```
{
  "data": [
    {
      "type": "appInfos",
      "id": "726ad1bb-3e1e-40eb-a986-d8a9897e4f1d",
      "attributes": {
        "appStoreState": "PREPARE_FOR_SUBMISSION",
        "appStoreAgeRating": "NINE_PLUS",
        "brazilAgeRating": "TEN",
        "kidsAgeBand": null
      },
      "relationships": {
        "app": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/app",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/app"
          }
        },
        "appInfoLocalizations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/appInfoLocalizations",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/appInfoLocalizations"
          }
        },
        "primaryCategory": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/primaryCategory",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/primaryCategory"
          }
        },
        "primarySubcategoryOne": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/primarySubcategoryOne",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/primarySubcategoryOne"
          }
        },
        "primarySubcategoryTwo": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/primarySubcategoryTwo",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/primarySubcategoryTwo"
          }
        },
        "secondaryCategory": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/secondaryCategory",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/secondaryCategory"
          }
        },
        "secondarySubcategoryOne": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/secondarySubcategoryOne",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/secondarySubcategoryOne"
          }
        },
        "secondarySubcategoryTwo": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/relationships/secondarySubcategoryTwo",
            "related": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d/secondarySubcategoryTwo"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appInfos/726ad1bb-3e1e-40eb-a986-d8a9897e4f1d"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/1462965264/appInfos"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}
```

## See Also

### Getting App Store details for your app

List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

GET /v1/apps/{id}/appStoreVersionExperimentsV2

