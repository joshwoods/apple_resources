

- App Store Server API
-  sendAttemptItem 

Object

# sendAttemptItem

The success or error information and the date the App Store server records when it attempts to send a server notification to your server.

App Store Server API 1.8+

``` source
object sendAttemptItem
```

## Properties

`attemptDate`

attemptDate

The date the App Store server attempts to send the notification.

`sendAttemptResult`

sendAttemptResult

The success or error information the App Store server records when it attempts to send an App Store server notification to your server.

## Mentioned in 

App Store Server API changelog

## Topics

### Data types

type attemptDate

The date the App Store server attempts to send a notification.

type sendAttemptResult

The success or error information the App Store server records when it attempts to send an App Store server notification to your server.

## See Also

### Data types

type signedPayload

A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.

