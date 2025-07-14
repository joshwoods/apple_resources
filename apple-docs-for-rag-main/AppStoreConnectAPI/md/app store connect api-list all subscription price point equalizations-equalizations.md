

- App Store Connect API
-  List All Subscription Price Point Equalizations 

Web Service Endpoint

# List All Subscription Price Point Equalizations

Get a list of subscription price points and their equivalent in a specified currency.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionPricePoints/{id}/equalizations
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, proceedsYear2, territory, equalizations`

`fields[territories]`

`[string]`

Value: `currency`

`filter[subscription]`

`[string]`

`filter[territory]`

`[string]`

`include`

`[string]`

Value: `territory`

`limit`

`integer`

Maximum: `8000`

## Response Codes

` 200 ``OK`

SubscriptionPricePointsResponse

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

## Mentioned in 

Managing auto-renewable subscriptions

## See Also

### Endpoints

Read Subscription Price Point Information

Get details about a specific subscription price point.

Create a Subscription Price Change

Schedule a subscription price change for a specific territory.

Delete Subscription Prices

Delete a scheduled price change for an auto-renewable subscription.

