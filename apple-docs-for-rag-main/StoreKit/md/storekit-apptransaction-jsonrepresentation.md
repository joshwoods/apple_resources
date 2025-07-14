

- StoreKit
- AppTransaction
-  jsonRepresentation 

Instance Property

# jsonRepresentation

The JSON representation of the app transaction information.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var jsonRepresentation: Data { get }
```

## Discussion

The jsonRepresentation is UTF-8 string data that contains the same information as the properties of the AppTransaction. You can use this JSON data to decode the app transaction information into your own data type instead of using AppTransaction properties directly.

The JSON Web Signature (JWS) Compact Serialization for the AppTransaction is available in the jwsRepresentation property of the VerificationResult. The JWS string consists of three Base64URL-encoded components, separated by a period: a header, a payload, and a signature. The jsonRepresentation is the Base64URL-decoded payload component.

Note

If you send the app transaction to your server or store it, use the jwsRepresentation and validate the signature before parsing it.

