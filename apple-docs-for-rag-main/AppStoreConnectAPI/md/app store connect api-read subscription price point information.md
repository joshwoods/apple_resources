

- App Store Connect API
-  Read Subscription Price Point Information 

Web Service Endpoint

# Read Subscription Price Point Information

Get details about a specific subscription price point.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionPricePoints/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, proceedsYear2, territory, equalizations`

`include`

`[string]`

Value: `territory`

## Response Codes

` 200 ``OK`

SubscriptionPricePointResponse

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

### Endpoints

List All Subscription Price Point Equalizations

Get a list of subscription price points and their equivalent in a specified currency.

Create a Subscription Price Change

Schedule a subscription price change for a specific territory.

Delete Subscription Prices

Delete a scheduled price change for an auto-renewable subscription.

