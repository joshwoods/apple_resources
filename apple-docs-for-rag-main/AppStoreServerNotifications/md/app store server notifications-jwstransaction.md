

- App Store Server Notifications
-  JWSTransaction 

Type

# JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

App Store Server Notifications 2.0+

``` source
string JWSTransaction
```

## Discussion

The JWSTransaction type is a string of three Base64URL-encoded components separated by a period. The string contains the JWS Compact Serialization of the transaction information, signed by the App Store according to the JSON Web Signature (JWS) IETF RFC 7515 specification.

The three components of the string are a header, a payload, and a signature, in that order.

- To read the transaction information, Base64URL-decode the payload. Use a JWSTransactionDecodedPayload object to read the payload information.

- To read the header, decode it and use a JWSDecodedHeader object to access the information. Use the information in the header to verify the signature.

### Use App Store Server Library functions

To verify a JWSTransaction on your server, consider implementing the verification using the App Store Server Library function `verifyAndDecodeTransaction`. The library provides this function in each language the library supports. For more information, see Simplifying your implementation by using the App Store Server Library.

## See Also

### JWS transaction and renewal info

type JWSRenewalInfo

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

object JWSRenewalInfoDecodedPayload

A decoded payload containing subscription renewal information for an auto-renewable subscription.

object JWSTransactionDecodedPayload

A decoded payload that contains transaction information.

