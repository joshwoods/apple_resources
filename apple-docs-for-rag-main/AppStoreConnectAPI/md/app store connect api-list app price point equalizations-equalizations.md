

- App Store Connect API
-  List app price point equalizations 

Web Service Endpoint

# List app price point equalizations

List all equivalent app prices points to a base price point.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v3/appPricePoints/{id}/equalizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app price point resource ID from the List all price points for an app response.

## Query Parameters

`fields[appPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, app, equalizations, territory`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[territories]`

`[string]`

Value: `currency`

`filter[territory]`

`[string]`

`include`

`[string]`

Possible Values: `app, territory`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AppPricePointsV3Response

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
https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDEifQ/equalizations?filter%5Bterritory%5D=USA,MEX&include=territory&fields%5BappPricePoints%5D=customerPrice,proceeds,territory&limit=5
```

```
{
  “data” : [ {
    “type” : “appPricePoints”,
    “id” : “eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJNRVgiLCJwIjoiMTAwMDEifQ”,
    “attributes” : {
      “customerPrice” : “19.0”,
      “proceeds” : “13.3”
    },
    “relationships” : {
      “territory” : {
        “data” : {
          “type” : “territories”,
          “id” : “MEX”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJNRVgiLCJwIjoiMTAwMDEifQ”
    }
  }, {
    “type” : “appPricePoints”,
    “id” : “eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDEifQ”,
    “attributes” : {
      “customerPrice” : “0.29”,
      “proceeds” : “0.2”
    },
    “relationships” : {
      “territory” : {
        “data” : {
          “type” : “territories”,
          “id” : “USA”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDEifQ”
    }
  } ],
  “included” : [ {
    “type” : “territories”,
    “id” : “MEX”,
    “attributes” : {
      “currency” : “MXN”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/territories/MEX”
    }
  }, {
    “type” : “territories”,
    “id” : “USA”,
    “attributes” : {
      “currency” : “USD”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/territories/USA”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDEifQ/equalizations?include=territory&fields%5BappPricePoints%5D=proceeds%2CcustomerPrice%2Cterritory&filter%5Bterritory%5D=MEX%2CUSA&limit=5”
  },
  “meta” : {
    “paging” : {
      “total” : 2,
      “limit” : 5
    }
  }
}

```

## See Also

### Getting an app’s price points

List all price points for an app

Get all the available price points for a specific app.

Read app price point information

Get details about a specific app price point.

