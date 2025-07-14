

- App Store Connect API
-  Modify a Promotional Offer 

Web Service Endpoint

# Modify a Promotional Offer

Update the prices for a specific promotional offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/subscriptionPromotionalOffers/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

SubscriptionPromotionalOfferUpdateRequest

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Endpoints

Create a Promotional Offer

Create a promotional offer for an auto-renewable subscription.

List All Promotional Offer Prices for a Subscription

Get a list of prices of a promotional offer for an auto-renewable subscription, for a specified territory.

Read Promotional Offer Information

Get details about a specific promotional offer for an auto-renewable subscription.

Delete a Promotional Offer from a Subscription

Delete a specific promotional offer from an auto-renewable subscription.

