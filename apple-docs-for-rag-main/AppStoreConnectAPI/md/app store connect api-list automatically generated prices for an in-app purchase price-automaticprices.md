

- App Store Connect API
-  List automatically generated prices for an in-app purchase price 

Web Service Endpoint

# List automatically generated prices for an in-app purchase price

Get information about a price or prices automatically set based on a base territory for an in-app purchase price schedule.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules/{id}/automaticPrices
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[inAppPurchasePricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, territory, equalizations`

`fields[inAppPurchasePrices]`

`[string]`

Possible Values: `startDate, endDate, manual, inAppPurchasePricePoint, territory`

`include`

`[string]`

Possible Values: `inAppPurchasePricePoint, territory`

`limit`

`integer`

Maximum: `200`

`filter[territory]`

`[string]`

`fields[territories]`

`[string]`

Value: `currency`

## Response Codes

` 200 ``OK`

InAppPurchasePricesResponse

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

## See Also

### Endpoints

Read in-app purchase price schedule information

Get information about a specific scheduled price change for an in-app purchase.

Read price information for an in-app purchase price schedule

Get information about a set price or prices for an in-app purchase price schedule.

Add a scheduled price change to an in-app purchase

Create a scheduled price change for an in-app purchase.

Read the selected base territory for an in-app purchase price schedule

Get information about the selected base territory for an in-app purchase price schedule.

