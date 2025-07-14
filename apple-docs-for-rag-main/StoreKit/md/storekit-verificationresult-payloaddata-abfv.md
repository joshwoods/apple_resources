

- StoreKit
- VerificationResult
-  payloadData 

Instance Property

# payloadData

The payload component of the JWS subscription renewal information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var payloadData: Data { get }
```

Available when `SignedType` is `Product.SubscriptionInfo.RenewalInfo`.

## Discussion

This value is the same as the jsonRepresentation in Product.SubscriptionInfo.RenewalInfo.

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

var signedData: Data

The subscription renewal information data that the signature applies to.

var signatureData: Data

The signature component of the JWS subscription renewal information.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

