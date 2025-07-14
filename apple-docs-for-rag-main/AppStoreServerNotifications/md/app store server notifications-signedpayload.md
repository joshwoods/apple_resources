

- App Store Server Notifications
-  signedPayload 

Type

# signedPayload

A cryptographically signed payload, in JSON Web Signature (JWS) format, that contains the response body for a version 2 notification.

App Store Server Notifications 2.0+

``` source
string signedPayload
```

## Mentioned in 

Receiving App Store Server Notifications

## Discussion

The `signedPayload` is a string of three Base64URL-encoded components, separated by a period. The string contains a JWS representation of the notification response body, signed by the App Store according to the JSON Web Signature (JWS) IETF RFC 7515 specification.

The three components of the string are a header, a payload, and a signature, in that order.

To read the notification response body, Base64URL-decode the payload. Use a responseBodyV2DecodedPayload object to read the payload information.

To read the header, Base64URL-decode it and use a JWSDecodedHeader object to access the information. Use the information in the decoded header to verify the signature.

