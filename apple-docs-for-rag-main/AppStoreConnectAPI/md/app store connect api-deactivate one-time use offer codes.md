

- App Store Connect API
-  Deactivate One-Time Use Offer Codes 

Web Service Endpoint

# Deactivate One-Time Use Offer Codes

Deactivate a batch of one-time use offer codes for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodeOneTimeUseCodes/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

SubscriptionOfferCodeOneTimeUseCodeUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionOfferCodeOneTimeUseCodeResponse

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

### Managing One-Time Use Offer Codes

Create One-Time Use Offer Codes

Create one-time use codes for an auto-renewable subscription offer.

Read One-Time Use Offer Code Information

Get details about a specific one-time use offer code for an auto-renewable subscription.

List All One-Time Use Offer Codes for an Auto-Renewable Subscription

Get details about a one-time use code for a specific subscription offer for an auto-renewable subscription.

List One-Time Use Offer Code Values

Get a list of one-time use offer codes for an auto-renewable subscription in CSV format.

