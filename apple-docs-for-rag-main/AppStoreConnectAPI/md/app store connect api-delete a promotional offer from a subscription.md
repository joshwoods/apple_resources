

- App Store Connect API
-  Delete a Promotional Offer from a Subscription 

Web Service Endpoint

# Delete a Promotional Offer from a Subscription

Delete a specific promotional offer from an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptionPromotionalOffers/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Endpoints

Create a Promotional Offer

Create a promotional offer for an auto-renewable subscription.

List All Promotional Offer Prices for a Subscription

Get a list of prices of a promotional offer for an auto-renewable subscription, for a specified territory.

Read Promotional Offer Information

Get details about a specific promotional offer for an auto-renewable subscription.

Modify a Promotional Offer

Update the prices for a specific promotional offer for an auto-renewable subscription.

