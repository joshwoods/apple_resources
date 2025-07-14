

- App Store Connect API
-  Create Custom Offer Codes 

Web Service Endpoint

# Create Custom Offer Codes

Create custom offer codes for an auto-renewable subscription offer.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodeCustomCodes
```

## HTTP Body

SubscriptionOfferCodeCustomCodeCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionOfferCodeCustomCodeResponse

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

### Managing Custom Offer Codes

List All Custom Offer Codes for an Auto-Renewable Subscription

Get details about a custom code for a specific subscription offer for an auto-renewable subscription.

Read Custom Offer Code Information

Get details about a specific offer code for an auto-renewable subscription.

Deactivate Custom Offer Codes

Deactivate a batch of custom offer codes for an auto-renewable subscription.

