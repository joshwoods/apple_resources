

- App Store Server API
-  notificationHistoryResponseItem 

Object

# notificationHistoryResponseItem

The App Store server notification history record, including the signed notification payload and the result of the server’s first send attempt.

App Store Server API 1.5+

``` source
object notificationHistoryResponseItem
```

## Properties

`sendAttempts`

`[`sendAttemptItem`]`

An array of information the App Store server records for its attempts to send a notification to your server. The maximum number of entries in the array is six.

`signedPayload`

signedPayload

The cryptographically signed payload, in JSON Web Signature (JWS) format, containing the original response body of a version 2 notification. For more information, see signedPayload in App Store Server Notifications.

`firstSendAttemptResult`

`string`

Deprecated 

The result of the App Store server’s first attempt to send the notification to your server’s App Store Server Notifications V2 endpoint.

Use the earliest sendAttemptItem in the `sendAttempts` array instead.

## Mentioned in 

App Store Server API changelog

## Topics

### Data types

type sendAttemptResult

The success or error information the App Store server records when it attempts to send an App Store server notification to your server.

object sendAttemptItem

The success or error information and the date the App Store server records when it attempts to send a server notification to your server.

type signedPayload

A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.

## See Also

### App Store Server Notifications history

Get Notification History

Get a list of notifications that the App Store server attempted to send to your server.

object NotificationHistoryRequest

The request body for notification history.

object NotificationHistoryResponse

A response that contains the App Store Server Notifications history for your app.

