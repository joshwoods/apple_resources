

- StoreKit
- VerificationResult
-  jwsRepresentation 

Instance Property

# jwsRepresentation

The app transaction signed by the App Store, in JWS Compact Serialization format.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var jwsRepresentation: String { get }
```

Available when `SignedType` is `AppTransaction`.

## Discussion

Use this JSON Web Signature (JWS) value to perform your own JWS verification on your server or on the device.

To verify the jwsRepresentation on your server, consider using the App Store Server Library function `verifyAndDecodeAppTransaction`, available in each language the library supports. For more information, see Simplifying your implementation by using the App Store Server Library.

The jwsRepresentation’s decoded payload contains the fields `deviceVerification` and `deviceVerificationNonce`. Use these fields on the device to verify that the JWS information belongs to the device. For more information, see deviceVerificationID.

## See Also

### Getting properties for app transactions

var deviceVerification: Data

The device verification value to use to verify whether the app transaction belongs to the device.

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

