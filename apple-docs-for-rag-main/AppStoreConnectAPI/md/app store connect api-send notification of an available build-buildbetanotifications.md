

- App Store Connect API
-  Send Notification of an Available Build 

Web Service Endpoint

# Send Notification of an Available Build

Send a notification to all assigned beta testers that a build is available for testing.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/buildBetaNotifications
```

## HTTP Body

BuildBetaNotificationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BuildBetaNotificationResponse

`Created`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

