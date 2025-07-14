

- App Store Server Notifications
-  responseBodyV2 

Object

# responseBodyV2

The response body the App Store sends in a version 2 server notification.

App Store Server Notifications 2.0+

``` source
object responseBodyV2
```

## Properties

`signedPayload`

signedPayload

The payload in JSON Web Signature (JWS) format, signed by the App Store.

## Mentioned in 

Receiving App Store Server Notifications

App Store Server Notifications changelog

## Discussion

The `signedPayload` object is a JWS representation. To get the transaction and subscription renewal details from the notification payload, process the `signedPayload` as follows:

1.  Parse `signedPayload` to identify the JWS header, payload, and signature representations.

2.  Base64URL-decode the payload to get the responseBodyV2DecodedPayload. The decoded payload contains details of the notification such as the notification type and data.

3.  The `data` object contains a `signedTransactionInfo` (JWSTransaction) and based on the notification type, a `signedRenewalInfo` (JWSRenewalInfo). Parse and Base64URL-decode these signed JWS representations to get transaction and subscription renewal details.

Each of the signed JWS representations, `signedPayload`, `signedTransactionInfo`, and `signedRenewalInfo`, have a JWS signature that you can validate on your server. Use the algorithm specified in the header’s alg parameter to validate the signature. For more information about validating signatures, see the JSON Web Signature (JWS) IETF RFC 7515 specification.

## Topics

### Response body payload

type signedPayload

A cryptographically signed payload, in JSON Web Signature (JWS) format, that contains the response body for a version 2 notification.

## See Also

### Server notifications version 2

App Store Server Notifications V2

Specify your secure server’s URL in App Store Connect to receive version 2 notifications.

object responseBodyV2DecodedPayload

A decoded payload that contains the version 2 notification data.

type notificationType

The type that describes the in-app purchase or external purchase event for which the App Store sends the version 2 notification.

type subtype

A string that provides details about select notification types in version 2.

