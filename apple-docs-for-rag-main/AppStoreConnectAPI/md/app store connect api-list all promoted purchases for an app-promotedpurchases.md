

- App Store Connect API
-  List All Promoted Purchases for an App 

Web Service Endpoint

# List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/promotedPurchases
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[inAppPurchases]`

`[string]`

Possible Values: `name, productId, inAppPurchaseType, state, reviewNote, familySharable, contentHosting, inAppPurchaseLocalizations, pricePoints, content, appStoreReviewScreenshot, promotedPurchase, iapPriceSchedule, inAppPurchaseAvailability, images`

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`fields[subscriptions]`

`[string]`

Possible Values: `name, productId, familySharable, state, subscriptionPeriod, reviewNote, groupLevel, subscriptionLocalizations, appStoreReviewScreenshot, group, introductoryOffers, promotionalOffers, offerCodes, prices, pricePoints, promotedPurchase, subscriptionAvailability, winBackOffers, images`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `inAppPurchaseV2, subscription`

`limit`

`integer`

The number of Promoted Purchases resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

PromotedPurchasesResponse

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

Managing auto-renewable subscriptions

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/1000001234/promotedPurchases
```

```
{
  "data": [
    {
      "type": "promotedPurchases",
      "id": "bec0022d-99b1-69b6-7524-e051b51f1976",
      "attributes": {
        "visibleForAllUsers": true,
        "enabled": true,
        "state": "APPROVED"
      },
      "relationships": {
        "promotionImages": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/bec0022d-99b1-69b6-7524-e051b51f1976/relationships/promotionImages",
            "related": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/bec0022d-99b1-69b6-7524-e051b51f1976/promotionImages"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/bec0022d-99b1-69b6-7524-e051b51f1976"
      }
    },
    {
      "type": "promotedPurchases",
      "id": "c5eb5306-0c66-eb2f-ee6a-7f4100536144",
      "attributes": {
        "visibleForAllUsers": true,
        "enabled": false,
        "state": "PREPARE_FOR_SUBMISSION"
      },
      "relationships": {
        "promotionImages": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/c5eb5306-0c66-eb2f-ee6a-7f4100536144/relationships/promotionImages",
            "related": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/c5eb5306-0c66-eb2f-ee6a-7f4100536144/promotionImages"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/promotedPurchases/c5eb5306-0c66-eb2f-ee6a-7f4100536144"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/1000001234/promotedPurchases"
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

### Getting in-app purchase information

Read In-App Purchase Information

Get information about an in-app purchase.

Deprecated

List All In-App Purchases for an App V1

List the in-app purchases that are available for your app.

Deprecated

