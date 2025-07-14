

- App Store Connect API
-  Create a Subscription Price Change 

Web Service Endpoint

# Create a Subscription Price Change

Schedule a subscription price change for a specific territory.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionPrices
```

## HTTP Body

SubscriptionPriceCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionPriceResponse

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

## Mentioned in 

Managing auto-renewable subscriptions

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Read Subscription Price Point Information

Get details about a specific subscription price point.

List All Subscription Price Point Equalizations

Get a list of subscription price points and their equivalent in a specified currency.

Delete Subscription Prices

Delete a scheduled price change for an auto-renewable subscription.

