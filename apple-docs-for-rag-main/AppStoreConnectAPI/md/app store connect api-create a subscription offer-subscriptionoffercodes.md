

- App Store Connect API
-  Create a Subscription Offer 

Web Service Endpoint

# Create a Subscription Offer

Create a subscription offer that provides offer codes for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodes
```

## HTTP Body

SubscriptionOfferCodeCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionOfferCodeResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating and Managing Subscription Offers

Read Subscription Offer Code Information

Get details about a specific subscription offer that has offer codes for an auto-renewable subscription.

Deactivate a Subscription Offer with Offer Codes

Deactivate a subscription offer that has offer codes for an auto-renewable subscription.

List All Subscription Offer Code Prices

Get a list of price tiers for a subscription offer code.

