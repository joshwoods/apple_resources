

- App Store Connect API
-  Read price schedule information for an app 

Web Service Endpoint

# Read price schedule information for an app

Read price schedule details for a specific app.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appPriceSchedule
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appPriceSchedules]`

`[string]`

Possible Values: `app, baseTerritory, manualPrices, automaticPrices`

`fields[appPrices]`

`[string]`

Possible Values: `manual, startDate, endDate, appPricePoint, territory`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[territories]`

`[string]`

Value: `currency`

`include`

`[string]`

Possible Values: `app, baseTerritory, manualPrices, automaticPrices`

`limit[automaticPrices]`

`integer`

Maximum: `50`

`limit[manualPrices]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppPriceScheduleResponse

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

## Mentioned in 

App Store Connect API 2.3 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6447402192/appPriceSchedule
```

```
{
  "data" : {
    "type" : "appPriceSchedules",
    "id" : "6447402192",
    "relationships" : {
      "baseTerritory" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/relationships/baseTerritory",
          "related" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/baseTerritory"
        }
      },
      "manualPrices" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/relationships/manualPrices",
          "related" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/manualPrices"
        }
      },
      "automaticPrices" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/relationships/automaticPrices",
          "related" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/automaticPrices"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/apps/6447402192/appPriceSchedule"
  }
}
```

## See Also

### Getting and managing an app’s price schedules

Read an app's price schedule information

List the price schedule details for a specific app.

List automatically generated prices for an app

List the automatically calculated prices for an app generated from a base territory.

Read the base territory for an app's price schedule

Read the base territory and currency for a specific app.

List manually chosen prices for an app

List the prices you chose for a specific app.

Add a scheduled price change to an app

Create a scheduled price change for an app.

