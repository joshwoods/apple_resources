

- App Store Connect API
-  List All Subscription Offer Code Prices 

Web Service Endpoint

# List All Subscription Offer Code Prices

Get a list of price tiers for a subscription offer code.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodes/{id}/prices
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionOfferCodePrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`fields[subscriptionPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, proceedsYear2, territory, equalizations`

`fields[territories]`

`[string]`

Value: `currency`

`include`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`limit`

`integer`

Maximum: `200`

`filter[territory]`

`[string]`

## Response Codes

` 200 ``OK`

SubscriptionOfferCodePricesResponse

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

### Creating and Managing Subscription Offers

Create a Subscription Offer

Create a subscription offer that provides offer codes for an auto-renewable subscription.

Read Subscription Offer Code Information

Get details about a specific subscription offer that has offer codes for an auto-renewable subscription.

Deactivate a Subscription Offer with Offer Codes

Deactivate a subscription offer that has offer codes for an auto-renewable subscription.

