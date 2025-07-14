

- App Store Connect API
-  List All Price Points for a Subscription 

Web Service Endpoint

# List All Price Points for a Subscription

Get a list of price points for an auto-renewable subscription by territory.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptions/{id}/pricePoints
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

`filter[territory]`

`[string]`

Use this filter with all requests.

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

App Store Connect API 2.4 release notes

App Store Connect API 3.6 release notes

### Discussion

Important

Use the `territory` filter on all requests. This will be required in a future release.

## See Also

### Endpoints

Create an Auto-Renewable Subscription

Create an auto-renewable subscription for your app.

Read Subscription Information

Get information about a specific auto-renewable subscription.

Modify an Auto-Renewable Subscription

Update a specific auto-renewable subscription.

Delete a Subscription

Delete a specific auto-renewable subscription that you configured for an app.

List All Localizations for an Auto-Renewable Subscription

Get a list of the subscription localizations for a specific auto-renewable subscription.

List All Introductory Offers for a Subscription

Get a list of introductory offers for a specific auto-renewable subscription.

List All Introductory Offer Resource IDs for an Auto-Renewable Subscription

Get a list of resource IDs representing introductory offers for an auto-renewable subscription.

Delete an Introductory Offer from a Subscription

Delete a specific introductory offer for an auto-renewable subscription.

Read Promoted Purchase Information for a Subscription

Get details about the promoted purchase of an auto-renewable subscription.

List All Offer Codes for a Subscription

Get a list of subscription offer codes for a specific auto-renewable subscription.

List All Promotional Offer Resource IDs for an Auto-Renewable Subscription

Get a list of promotional offers for a specific auto-renewable subscription.

List All Prices for a Subscription

Get a list of prices for an auto-renewable subscription, by territory.

List All Subscription Prices IDs for an Auto-Renewable Subscription

Get a list of resource IDs representing subscription prices for an auto-renewable subscription.

Delete Prices from a Subscription

Delete a scheduled subscription price change for an auto-renewable subscription.

Read Review Screenshot Information for a Subscription

Get information about review screenshot for a specific auto-renewable subscription.

