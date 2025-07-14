

- StoreKit
- Transaction
-  jsonRepresentation 

Instance Property

# jsonRepresentation

The JSON representation of the transaction information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var jsonRepresentation: Data { get }
```

## Discussion

The jsonRepresentation is UTF-8 string data that has the same JSON schema as the JWSTransactionDecodedPayload object. You can use this data to decode the transaction information into your own data type instead of using the Transaction value and its Transaction properties directly.

The JSON Web Signature (JWS) Compact Serialization for the transaction is available in the jwsRepresentation property of the VerificationResult. The JWS string consists of three Base64URL-encoded components, separated by a period: a header, a payload, and a signature. The jsonRepresentation is the Base64URL-decoded payload component.

Note

If you send the transaction to your server or store it, use the jwsRepresentation and validate the signature before parsing it.

