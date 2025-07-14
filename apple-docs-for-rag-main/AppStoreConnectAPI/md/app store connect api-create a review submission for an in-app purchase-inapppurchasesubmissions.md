

- App Store Connect API
-  Create a Review Submission for an In-App Purchase 

Web Service Endpoint

# Create a Review Submission for an In-App Purchase

Create an in-app purchase submission for review.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/inAppPurchaseSubmissions
```

## HTTP Body

InAppPurchaseSubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

InAppPurchaseSubmissionResponse

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

