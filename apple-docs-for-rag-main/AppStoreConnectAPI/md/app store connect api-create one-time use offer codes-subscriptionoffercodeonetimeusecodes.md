

- App Store Connect API
-  Create One-Time Use Offer Codes 

Web Service Endpoint

# Create One-Time Use Offer Codes

Create one-time use codes for an auto-renewable subscription offer.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodeOneTimeUseCodes
```

## HTTP Body

SubscriptionOfferCodeOneTimeUseCodeCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionOfferCodeOneTimeUseCodeResponse

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

### Managing One-Time Use Offer Codes

Read One-Time Use Offer Code Information

Get details about a specific one-time use offer code for an auto-renewable subscription.

Deactivate One-Time Use Offer Codes

Deactivate a batch of one-time use offer codes for an auto-renewable subscription.

List All One-Time Use Offer Codes for an Auto-Renewable Subscription

Get details about a one-time use code for a specific subscription offer for an auto-renewable subscription.

List One-Time Use Offer Code Values

Get a list of one-time use offer codes for an auto-renewable subscription in CSV format.

