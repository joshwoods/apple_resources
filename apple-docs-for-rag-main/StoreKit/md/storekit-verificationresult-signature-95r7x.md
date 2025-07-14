

- StoreKit
- VerificationResult
-  signature 

Instance Property

# signature

The signature component of the JSON web signature.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var signature: P256.Signing.ECDSASignature { get }
```

Available when `SignedType` is `Product.SubscriptionInfo.RenewalInfo`.

## Discussion

Use this signature with Apple CryptoKit if you verify the signature on the device.

## See Also

### Getting properties for subscription renewal information

var jwsRepresentation: String

The subscription renewal information signed by the App Store, in JWS Compact Serialization format.

var deviceVerification: Data

The device verification value to use to verify whether the subscription renewal information belongs to the device.

var deviceVerificationNonce: UUID

The UUID for computing the device verification value.

var signedDate: Date

The date that the App Store signed the JWS subscription renewal information.

var headerData: Data

The header component of the JWS subscription renewal information.

var payloadData: Data

The payload component of the JWS subscription renewal information.

var signedData: Data

The subscription renewal information data that the signature applies to.

var signatureData: Data

The signature component of the JWS subscription renewal information.

