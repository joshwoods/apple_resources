

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  jsonRepresentation 

Instance Property

# jsonRepresentation

The JSON representation of the subscription renewal information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var jsonRepresentation: Data { get }
```

## Discussion

The jsonRepresentation is UTF-8 string data that has the same JSON schema as the JWSRenewalInfoDecodedPayload object. You can use the JSON data to decode the subscription renewal information into your own data type, or use the Product.SubscriptionInfo.RenewalInfo value and its properties directly.

The JSON Web Signature (JWS) Compact Serialization for the subscription renewal information is available in the jwsRepresentation property of the VerificationResult. The JWS string consists of three Base64URL-encoded components, separated by a period: a header, a payload, and a signature. The jsonRepresentation is the Base64URL-decoded payload component.

Note

If you send the subscription renewal information to your server or store it, use the jwsRepresentation and validate the signature before parsing it.

