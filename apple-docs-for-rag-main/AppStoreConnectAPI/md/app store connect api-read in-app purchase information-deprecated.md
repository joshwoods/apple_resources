

- App Store Connect API
-  Read In-App Purchase Information Deprecated

Web Service Endpoint

# Read In-App Purchase Information

Get information about an in-app purchase.

App Store Connect API 1.2–3.0Deprecated

Deprecated

Use Read In-App Purchase Information instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[inAppPurchases]`

`[string]`

Possible Values: `referenceName, productId, inAppPurchaseType, state, apps`

`include`

`[string]`

Value: `apps`

`limit[apps]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

InAppPurchaseResponse

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

Managing in-app purchases

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/inAppPurchases/6446998023
```

```
{
  "data": [
    {
      "type": "inAppPurchases",
      "id": "6447027998",
      "attributes": {
        "name": "YNC1",
        "productId": "YNCNC1",
        "inAppPurchaseType": "NON_CONSUMABLE",
        "state": "MISSING_METADATA",
        "reviewNote": null,
        "familySharable": false,
        "contentHosting": false,
        "availableInAllTerritories": true
      },
      "relationships": {
        "inAppPurchaseLocalizations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/inAppPurchaseLocalizations",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/inAppPurchaseLocalizations"
          }
        },
        "pricePoints": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/pricePoints",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/pricePoints"
          }
        },
        "content": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/content",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/content"
          }
        },
        "appStoreReviewScreenshot": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/appStoreReviewScreenshot",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/appStoreReviewScreenshot"
          }
        },
        "promotedPurchase": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/promotedPurchase",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/promotedPurchase"
          }
        },
        "iapPriceSchedule": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/relationships/iapPriceSchedule",
            "related": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998/iapPriceSchedule"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v2/inAppPurchases/6447027998"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/inAppPurchasesV2"
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

List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

List All In-App Purchases for an App V1

List the in-app purchases that are available for your app.

Deprecated

