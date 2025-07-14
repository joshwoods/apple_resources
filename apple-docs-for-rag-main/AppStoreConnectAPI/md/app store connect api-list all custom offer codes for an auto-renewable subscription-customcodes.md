

- App Store Connect API
-  List All Custom Offer Codes for an Auto-Renewable Subscription 

Web Service Endpoint

# List All Custom Offer Codes for an Auto-Renewable Subscription

Get details about a custom code for a specific subscription offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodes/{id}/customCodes
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionOfferCodeCustomCodes]`

`[string]`

Possible Values: `customCode, numberOfCodes, createdDate, expirationDate, active, offerCode`

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

SubscriptionOfferCodeCustomCodesResponse

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

### Managing Custom Offer Codes

Create Custom Offer Codes

Create custom offer codes for an auto-renewable subscription offer.

Read Custom Offer Code Information

Get details about a specific offer code for an auto-renewable subscription.

Deactivate Custom Offer Codes

Deactivate a batch of custom offer codes for an auto-renewable subscription.

