

- App Store Connect API
-  Read Promotional Offer Information 

Web Service Endpoint

# Read Promotional Offer Information

Get details about a specific promotional offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionPromotionalOffers/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionPromotionalOfferPrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`fields[subscriptionPromotionalOffers]`

`[string]`

Possible Values: `name, offerCode, duration, offerMode, numberOfPeriods, subscription, prices`

`include`

`[string]`

Possible Values: `subscription, prices`

`limit[prices]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

SubscriptionPromotionalOfferResponse

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

List All Promotional Offer Prices for a Subscription

Get a list of prices of a promotional offer for an auto-renewable subscription, for a specified territory.

Modify a Promotional Offer

Update the prices for a specific promotional offer for an auto-renewable subscription.

Delete a Promotional Offer from a Subscription

Delete a specific promotional offer from an auto-renewable subscription.

