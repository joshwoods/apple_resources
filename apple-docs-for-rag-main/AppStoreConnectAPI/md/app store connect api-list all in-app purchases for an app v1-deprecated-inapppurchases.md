

- App Store Connect API
-  List All In-App Purchases for an App V1 Deprecated

Web Service Endpoint

# List All In-App Purchases for an App V1

List the in-app purchases that are available for your app.

App Store Connect API 1.2–2.0Deprecated

Deprecated

Use List All In-App Purchases for an App instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/inAppPurchases
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[inAppPurchases]`

`[string]`

Possible Values: `referenceName, productId, inAppPurchaseType, state, apps`

`filter[canBeSubmitted]`

`[string]`

`filter[inAppPurchaseType]`

`[string]`

Possible Values: `AUTOMATICALLY_RENEWABLE_SUBSCRIPTION, NON_CONSUMABLE, CONSUMABLE, NON_RENEWING_SUBSCRIPTION, FREE_SUBSCRIPTION`

`include`

`[string]`

Value: `apps`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `referenceName, -referenceName, productId, -productId, inAppPurchaseType, -inAppPurchaseType`

`limit[apps]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

InAppPurchasesResponse

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

App Store Connect API 2.2 release notes

Managing in-app purchases

App Store Connect API 2.0 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023/inAppPurchases
```

```
{
    "data": [
        {
            "type": "inAppPurchases",
            "id": "ca38ea26-b7d5-4989-9615-c678cb05aabd",
            "attributes": {
                "referenceName": "YNC1",
                "productId": "YNCNC1",
                "inAppPurchaseType": "NON_CONSUMABLE",
                "state": "WAITING_FOR_SCREENSHOT"
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/inAppPurchases/ca38ea26-b7d5-4989-9615-c678cb05aabd"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/inAppPurchases"
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

### Getting in-app purchase information

Read In-App Purchase Information

Get information about an in-app purchase.

Deprecated

List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

