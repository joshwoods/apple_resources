

- App Store Server API
-  signedPayload 

Type

# signedPayload

A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.

App Store Server API 1.5+

``` source
string signedPayload
```

## Discussion

The `signedpayload` is a string of three Base64 URL-encoded components, separated by a period.

For more information, see signedPayload in App Store Server Notifications.

## See Also

### Data types

object sendAttemptItem

The success or error information and the date the App Store server records when it attempts to send a server notification to your server.

