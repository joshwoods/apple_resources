

- App Store Connect API
-  Create a Review Submission for a Subscription Group 

Web Service Endpoint

# Create a Review Submission for a Subscription Group

Create a subscription group submission for review.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionGroupSubmissions
```

## HTTP Body

SubscriptionGroupSubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionGroupSubmissionResponse

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

Submitting subscriptions and subscription groups for App Review

## See Also

### Endpoints

Create a Review Submission for a Subscription

Create a review submission for an auto-renewable subscription.

