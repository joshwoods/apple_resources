

- App Store Connect API
-  Read Subscription Offer Code Information 

Web Service Endpoint

# Read Subscription Offer Code Information

Get details about a specific subscription offer that has offer codes for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodes/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionOfferCodeCustomCodes]`

`[string]`

Possible Values: `customCode, numberOfCodes, createdDate, expirationDate, active, offerCode`

`fields[subscriptionOfferCodeOneTimeUseCodes]`

`[string]`

Possible Values: `numberOfCodes, createdDate, expirationDate, active, offerCode, values`

`fields[subscriptionOfferCodePrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`fields[subscriptionOfferCodes]`

`[string]`

Possible Values: `name, customerEligibilities, offerEligibility, duration, offerMode, numberOfPeriods, totalNumberOfCodes, active, subscription, oneTimeUseCodes, customCodes, prices`

`include`

`[string]`

Possible Values: `subscription, oneTimeUseCodes, customCodes, prices`

`limit[customCodes]`

`integer`

Maximum: `50`

`limit[oneTimeUseCodes]`

`integer`

Maximum: `50`

`limit[prices]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

SubscriptionOfferCodeResponse

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

### Creating and Managing Subscription Offers

Create a Subscription Offer

Create a subscription offer that provides offer codes for an auto-renewable subscription.

Deactivate a Subscription Offer with Offer Codes

Deactivate a subscription offer that has offer codes for an auto-renewable subscription.

List All Subscription Offer Code Prices

Get a list of price tiers for a subscription offer code.

