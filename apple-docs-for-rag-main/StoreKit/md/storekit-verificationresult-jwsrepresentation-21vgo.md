

- StoreKit
- VerificationResult
-  jwsRepresentation 

Instance Property

# jwsRepresentation

The transaction signed by the App Store, in JWS Compact Serialization format.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var jwsRepresentation: String { get }
```

Available when `SignedType` is `Transaction`.

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

Use this JSON Web Signature (JWS) value to perform your own JWS verification on your server or on the device.

The jwsRepresentation is the same as the JWSTransaction that the App Store Server API returns and the JWSTransaction that you receive from App Store Server Notifications. The jwsRepresentation’s decoded payload contains two additional fields: `deviceVerification` and `deviceVerificationNonce`. Use these fields on the device to verify that the JWS information belongs to the device. For more information, see deviceVerificationID.

To verify the jwsRepresentation on your server, consider using the App Store Server Library function `verifyAndDecodeTransaction`, available in each language the library supports. For more information, see Simplifying your implementation by using the App Store Server Library.

Important

The decoded payloads of the jwsRepresentation and JWSTransaction strings contain price fields that are specified in *milliunits* of the currency; StoreKit represents the `price` in *units* of currency. Take care not to confuse these two representations when working with both APIs.

## See Also

### Getting properties for transactions

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

var signedData: Data

The transaction data that the signature applies to.

var signatureData: Data

The signature component of the JWS transaction.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

