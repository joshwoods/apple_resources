

- StoreKit
- VerificationResult
-  deviceVerification 

Instance Property

# deviceVerification

The device verification value to use to verify whether the app transaction belongs to the device.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var deviceVerification: Data { get }
```

Available when `SignedType` is `AppTransaction`.

## Discussion

For more information about using the device verification value, see deviceVerification.

This value is identical to the deviceVerification value in AppTransaction.

## See Also

### Getting properties for app transactions

var jwsRepresentation: String

The app transaction signed by the App Store, in JWS Compact Serialization format.

var deviceVerificationNonce: UUID

The UUID for computing the device verification value.

var signedDate: Date

The date that the App Store signed the JWS app transaction.

var headerData: Data

The header component of the JWS app transaction.

var payloadData: Data

The payload component of the JWS app transaction.

var signedData: Data

The app transaction data that the signature applies to.

var signatureData: Data

The signature component of the JWS app transaction.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

