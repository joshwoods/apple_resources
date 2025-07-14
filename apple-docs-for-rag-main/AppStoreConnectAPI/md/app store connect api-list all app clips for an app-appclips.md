

- App Store Connect API
-  List All App Clips for an App 

Web Service Endpoint

# List All App Clips for an App

List your app’s associated App Clips.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appClips
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appClipDefaultExperiences]`

`[string]`

Additional fields to include for each App Clips resource returned by the response.

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`fields[appClips]`

`[string]`

Additional fields to include for each App Clips resource returned by the response.

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`filter[bundleId]`

`[string]`

Filter the returned App Clips using the bundle ID of the App Clip.

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `app, appClipDefaultExperiences`

`limit`

`integer`

The number of App Clips resources to return.

Maximum: `200`

`limit[appClipDefaultExperiences]`

`integer`

The number of included App Clips resources to return if the default App Clip experience localizations relationship is included.

Maximum: `50`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

AppClipsResponse

`OK`

The request completed successfully.

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
https://api.appstoreconnect.apple.comv1/apps/{id}/appClips
```

```
{
  "data": [
    {
      "type": "appClips",
      "id": "37453eec-75b3-4578-aba4-ah345936650",
      "attributes": {
        "bundleId": "com.domain.app.AppClip"
      },
      "relationships": {
        "appClipDefaultExperiences": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appClips/37453eec-75b3-4578-aba4-ah345936650/relationships/appClipDefaultExperiences",
            "related": "https://api.appstoreconnect.apple.com/v1/appClips/37453eec-75b3-4578-aba4-ah345936650/appClipDefaultExperiences"
          }
        },
        "appClipAdvancedExperiences": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appClips/37453eec-75b3-4578-aba4-ah345936650/relationships/appClipAdvancedExperiences",
            "related": "https://api.appstoreconnect.apple.com/v1/appClips/37453eec-75b3-4578-aba4-ah345936650/appClipAdvancedExperiences"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appClips/37453eec-75b3-4578-aba4-ah345936650"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/1000001234/appClips"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}
```

