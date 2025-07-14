

- App Store Connect API
-  Modify the territory availability of a subscription 

Web Service Endpoint

# Modify the territory availability of a subscription

Update the territory availability of a specific subscription.

App Store Connect API 2.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities
```

## HTTP Body

SubscriptionAvailabilityCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionAvailabilityResponse

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

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Read the availability of a subscription

Get information about the territory availability for a subscription.

List the territory availability of a subscription

List the territory availability and currency of a specific subscription.

