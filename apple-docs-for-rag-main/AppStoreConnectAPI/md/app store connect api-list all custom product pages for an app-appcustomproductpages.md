

- App Store Connect API
-  List all custom product pages for an app 

Web Service Endpoint

# List all custom product pages for an app

Get a list of all custom product pages for a specific app.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appCustomProductPages
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appCustomProductPageVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, state, deepLink, appCustomProductPage, appCustomProductPageLocalizations`

`fields[appCustomProductPages]`

`[string]`

Fields to return for included related types.

Possible Values: `name, url, visible, app, appCustomProductPageVersions`

`filter[visible]`

`[string]`

Fields to return for included related types.

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `app, appCustomProductPageVersions`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`limit[appCustomProductPageVersions]`

`integer`

Number of resources to return.

Maximum: `50`

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

AppCustomProductPagesResponse

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
https://api.appstoreconnect.apple.com/v1/apps/01234/appCustomProductPages
```

```
{
  "data": [
    {
      "type": "appCustomProductPages",
      "id": "eb2b3606-2fef-4aab-a54e-b2e5547c9bc3",
      "attributes": {
        "name": "Custom Product Page May 1",
        "url": "https://apps.apple.com/us/app/name/id01234?ppid=eb2b3606-2fef-4aab-a54e-b2e5547c9bc3",
        "visible": false
      },
      "relationships": {
        "appCustomProductPageVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3/relationships/appCustomProductPageVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3/appCustomProductPageVersions"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3"
      }
    },
    {
      "type": "appCustomProductPages",
      "id": "2a92bd8e-e59a-4b6e-bca0-04209c16fc7e",
      "attributes": {
        "name": "Customer Product Page 1",
        "url": "https://apps.apple.com/us/app/gersey-numba/id1526908970?ppid=2a92bd8e-e59a-4b6e-bca0-04209c16fc7e",
        "visible": true
      },
      "relationships": {
        "appCustomProductPageVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/2a92bd8e-e59a-4b6e-bca0-04209c16fc7e/relationships/appCustomProductPageVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/2a92bd8e-e59a-4b6e-bca0-04209c16fc7e/appCustomProductPageVersions"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appCustomProductPages/2a92bd8e-e59a-4b6e-bca0-04209c16fc7e"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/01234/appCustomProductPages"
  },
  "meta": {
    "paging": {
      "total": 2,
      "limit": 50
    }
  }
}
```

## See Also

### Getting App Store details for your app

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

GET /v1/apps/{id}/appStoreVersionExperimentsV2

