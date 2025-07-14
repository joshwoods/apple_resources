

- App Store Connect API
-  Read in-app purchase price schedule information 

Web Service Endpoint

# Read in-app purchase price schedule information

Get information about a specific scheduled price change for an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[inAppPurchasePriceSchedules]`

`[string]`

Possible Values: `baseTerritory, manualPrices, automaticPrices`

`fields[inAppPurchasePrices]`

`[string]`

Possible Values: `startDate, endDate, manual, inAppPurchasePricePoint, territory`

`include`

`[string]`

Possible Values: `baseTerritory, manualPrices, automaticPrices`

`limit[manualPrices]`

`integer`

Maximum: `50`

`fields[territories]`

`[string]`

Value: `currency`

`limit[automaticPrices]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

InAppPurchasePriceScheduleResponse

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
https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593
```

```
{
  "data" : {
    "type" : "inAppPurchasePriceSchedules",
    "id" : "6447501593",
    "relationships" : {
      "baseTerritory" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/relationships/baseTerritory",
          "related" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/baseTerritory"
        }
      },
      "manualPrices" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/relationships/manualPrices",
          "related" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/manualPrices"
        }
      },
      "automaticPrices" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/relationships/automaticPrices",
          "related" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593/automaticPrices"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/6447501593"
  }
}
```

## See Also

### Endpoints

Read price information for an in-app purchase price schedule

Get information about a set price or prices for an in-app purchase price schedule.

Add a scheduled price change to an in-app purchase

Create a scheduled price change for an in-app purchase.

List automatically generated prices for an in-app purchase price

Get information about a price or prices automatically set based on a base territory for an in-app purchase price schedule.

Read the selected base territory for an in-app purchase price schedule

Get information about the selected base territory for an in-app purchase price schedule.

