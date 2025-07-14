

- StoreKit
- VerificationResult
-  signedData 

Instance Property

# signedData

The transaction data that the signature applies to.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var signedData: Data { get }
```

Available when `SignedType` is `Transaction`.

## See Also

### Getting properties for transactions

var jwsRepresentation: String

The transaction signed by the App Store, in JWS Compact Serialization format.

var deviceVerification: Data

The device verification value to use to verify whether the transaction belongs to the device.

var deviceVerificationNonce: UUID

The UUID for computing the device verification value.

var signedDate: Date

The date that the App Store signed the JWS transaction.

var headerData: Data

The header component of the JWS transaction.

var payloadData: Data

The payload component of the JWS transaction.

var signatureData: Data

The signature component of the JWS transaction.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

