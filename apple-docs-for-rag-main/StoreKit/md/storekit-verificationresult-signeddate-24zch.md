

- StoreKit
- VerificationResult
-  signedDate 

Instance Property

# signedDate

The date that the App Store signed the JWS app transaction.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var signedDate: Date { get }
```

Available when `SignedType` is `AppTransaction`.

## Discussion

Use the signedDate to verify whether the certificate used to sign the transaction was valid when the App Store signed the transaction.

## See Also

### Getting properties for app transactions

var jwsRepresentation: String

The app transaction signed by the App Store, in JWS Compact Serialization format.

var deviceVerification: Data

The device verification value to use to verify whether the app transaction belongs to the device.

var deviceVerificationNonce: UUID

The UUID for computing the device verification value.

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

