

- App Store Connect API
-  List One-Time Use Offer Code Values 

Web Service Endpoint

# List One-Time Use Offer Code Values

Get a list of one-time use offer codes for an auto-renewable subscription in CSV format.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionOfferCodeOneTimeUseCodes/{id}/values
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 200 ``OK`

csv

`OK`

Content-Type: text/csv

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

List All One-Time Use Offer Codes for an Auto-Renewable Subscription

Get details about a one-time use code for a specific subscription offer for an auto-renewable subscription.

