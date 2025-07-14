

- App Store Connect API
-  Delete Subscription Prices 

Web Service Endpoint

# Delete Subscription Prices

Delete a scheduled price change for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptionPrices/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Read Subscription Price Point Information

Get details about a specific subscription price point.

List All Subscription Price Point Equalizations

Get a list of subscription price points and their equivalent in a specified currency.

Create a Subscription Price Change

Schedule a subscription price change for a specific territory.

