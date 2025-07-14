

- App Store Connect API
-  List All One-Time Use Offer Codes for an Auto-Renewable Subscription 

Web Service Endpoint

# List All One-Time Use Offer Codes for an Auto-Renewable Subscription

Get details about a one-time use code for a specific subscription offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodes/{id}/oneTimeUseCodes
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionOfferCodeOneTimeUseCodes]`

`[string]`

Possible Values: `numberOfCodes, createdDate, expirationDate, active, offerCode, values`

`fields[subscriptionOfferCodes]`

`[string]`

Possible Values: `name, customerEligibilities, offerEligibility, duration, offerMode, numberOfPeriods, totalNumberOfCodes, active, subscription, oneTimeUseCodes, customCodes, prices`

`include`

`[string]`

Value: `offerCode`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

SubscriptionOfferCodeOneTimeUseCodesResponse

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

### Managing One-Time Use Offer Codes

Create One-Time Use Offer Codes

Create one-time use codes for an auto-renewable subscription offer.

Read One-Time Use Offer Code Information

Get details about a specific one-time use offer code for an auto-renewable subscription.

Deactivate One-Time Use Offer Codes

Deactivate a batch of one-time use offer codes for an auto-renewable subscription.

List One-Time Use Offer Code Values

Get a list of one-time use offer codes for an auto-renewable subscription in CSV format.

