

- App Store Server API
-  Get Test Notification Status 

Web Service Endpoint

# Get Test Notification Status

Check the status of the test App Store server notification sent to your server.

App Store Server API 1.5+

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/notifications/test/{testNotificationToken}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test/{testNotificationToken}
```

## Path Parameters

`testNotificationToken`

testNotificationToken

 (Required) 

The token that uniquely identifies a test, that you receive when you call Request a Test Notification.

## Response Codes

` 200 ``OK`

CheckTestNotificationResponse

`OK`

Success.

Content-Type: application/json

` 400 ``Bad Request`

InvalidTestNotificationTokenError

`Bad Request`

The test notification token is invalid. Use a valid token that you receive in the SendTestNotificationResponse.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 404 ``Not Found`

TestNotificationNotFoundError

`Not Found`

The status isn’t yet available or the test notification token wasn’t found.

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Server error. Try again later.

Content-Type: application/json

## Mentioned in 

App Store Server API changelog

Identifying rate limits

## Discussion

Call this endpoint using the testNotificationToken you receive when you call Request a Test Notification. You can check the status using the testNotificationToken for up to six months. Use the information in the CheckTestNotificationResponse to troubleshoot your server if it’s unable to receive App Store Server Notifications successfully.

## See Also

### App Store Server Notifications testing

Request a Test Notification

Ask App Store Server Notifications to send a test notification to your server.

object SendTestNotificationResponse

A response that contains the test notification token.

object CheckTestNotificationResponse

A response that contains the contents of the App Store server’s test notification and the result from your server.

