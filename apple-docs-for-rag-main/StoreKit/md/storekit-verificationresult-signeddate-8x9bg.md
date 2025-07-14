

- StoreKit
- VerificationResult
-  signedDate 

Instance Property

# signedDate

The date that the App Store signed the JWS transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var signedDate: Date { get }
```

Available when `SignedType` is `Transaction`.

## Discussion

Use the signedDate to verify whether the certificate used to sign the transaction was valid when the App Store signed the transaction.

## See Also

### Getting properties for transactions

var jwsRepresentation: String

The transaction signed by the App Store, in JWS Compact Serialization format.

var deviceVerification: Data

The device verification value to use to verify whether the transaction belongs to the device.

var deviceVerificationNonce: UUID

The UUID for computing the device verification value.

var headerData: Data

The header component of the JWS transaction.

var payloadData: Data

The payload component of the JWS transaction.

var signedData: Data

The transaction data that the signature applies to.

var signatureData: Data

The signature component of the JWS transaction.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

