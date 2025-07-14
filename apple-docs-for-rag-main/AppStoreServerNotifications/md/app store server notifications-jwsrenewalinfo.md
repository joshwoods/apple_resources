

- App Store Server Notifications
-  JWSRenewalInfo 

Type

# JWSRenewalInfo

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

App Store Server Notifications 2.0+

``` source
string JWSRenewalInfo
```

## Discussion

The JWSRenewalInfo type is a string of three Base64 URL-encoded components, separated by a period. The string contains the JWS representation of the subscription renewal information, signed by the App Store according to the JSON Web Signature (JWS) IETF RFC 7515 specification.

The three components in the string are a header, a payload, and a signature, in that order.

To read the subscription renewal information, Base64 URL-decode the payload. Use a JWSRenewalInfoDecodedPayload object to read the payload information.

To read the header, Base64 URL-decode it and use a JWSDecodedHeader object to access the information. Use the information in the header to verify the signature.

## See Also

### JWS transaction and renewal info

object JWSRenewalInfoDecodedPayload

A decoded payload containing subscription renewal information for an auto-renewable subscription.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

object JWSTransactionDecodedPayload

A decoded payload that contains transaction information.

