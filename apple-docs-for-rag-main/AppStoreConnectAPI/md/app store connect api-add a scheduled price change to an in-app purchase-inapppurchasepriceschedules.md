

- App Store Connect API
-  Add a scheduled price change to an in-app purchase 

Web Service Endpoint

# Add a scheduled price change to an in-app purchase

Create a scheduled price change for an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/inAppPurchasePriceSchedules
```

## HTTP Body

InAppPurchasePriceScheduleCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

InAppPurchasePriceScheduleResponse

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

Managing in-app purchases

## Discussion

Note

A base territory is now required when adding or creating a price for an in-app purchase.

## See Also

### Endpoints

Read in-app purchase price schedule information

Get information about a specific scheduled price change for an in-app purchase.

Read price information for an in-app purchase price schedule

Get information about a set price or prices for an in-app purchase price schedule.

List automatically generated prices for an in-app purchase price

Get information about a price or prices automatically set based on a base territory for an in-app purchase price schedule.

Read the selected base territory for an in-app purchase price schedule

Get information about the selected base territory for an in-app purchase price schedule.

