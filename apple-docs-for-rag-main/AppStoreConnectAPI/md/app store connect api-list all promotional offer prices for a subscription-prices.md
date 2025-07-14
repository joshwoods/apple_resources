

- App Store Connect API
-  List All Promotional Offer Prices for a Subscription 

Web Service Endpoint

# List All Promotional Offer Prices for a Subscription

Get a list of prices of a promotional offer for an auto-renewable subscription, for a specified territory.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionPromotionalOffers/{id}/prices
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, proceedsYear2, territory, equalizations`

`fields[subscriptionPromotionalOfferPrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

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

SubscriptionPromotionalOfferPricesResponse

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

Create a Promotional Offer

Create a promotional offer for an auto-renewable subscription.

Read Promotional Offer Information

Get details about a specific promotional offer for an auto-renewable subscription.

Modify a Promotional Offer

Update the prices for a specific promotional offer for an auto-renewable subscription.

Delete a Promotional Offer from a Subscription

Delete a specific promotional offer from an auto-renewable subscription.

