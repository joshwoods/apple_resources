

- App Store Connect API
-  Read Custom Offer Code Information 

Web Service Endpoint

# Read Custom Offer Code Information

Get details about a specific offer code for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodeCustomCodes/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionOfferCodeCustomCodes]`

`[string]`

Possible Values: `customCode, numberOfCodes, createdDate, expirationDate, active, offerCode`

`include`

`[string]`

Value: `offerCode`

## Response Codes

` 200 ``OK`

SubscriptionOfferCodeCustomCodeResponse

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

List All Custom Offer Codes for an Auto-Renewable Subscription

Get details about a custom code for a specific subscription offer for an auto-renewable subscription.

Deactivate Custom Offer Codes

Deactivate a batch of custom offer codes for an auto-renewable subscription.

