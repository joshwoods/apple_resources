

- StoreKit
-  VerificationResult 

Enumeration

# VerificationResult

A type that describes the result of a StoreKit verification.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum VerificationResult
```

## Overview

StoreKit automatically verifies the Transaction, Product.SubscriptionInfo.RenewalInfo, and AppTransaction values. To access the wrapped values, check whether the values are verified or unverified.

In addition to getting a verification result from StoreKit, you might want to verify the signed information yourself, either on the device, or on your server for the most control and security. Perform the verification on the jwsRepresentation property for subscription renewal information, the jwsRepresentation property for transactions, and the jwsRepresentation property for an app transaction.

To verify the jwsRepresentation on your server, consider using the verification functions in the App Store Server Library. The library provides the functions `verifyAndDecodeTransaction`, `verifyAndDecodeAppTransaction`, and `verifyAndDecodeRenewalInfo` in each language the library supports. For more information, see Simplifying your implementation by using the App Store Server Library.

The jwsRepresentation string is in JWS Compact Serialization format and is the same as its counterpart in the App Store server APIs, as follows:

| StoreKit string | Equivalent in the App Store Server API | Equivalent in App Store Server Notifications |
|----|----|----|
| jwsRepresentation for subscription renewal information | JWSRenewalInfo | JWSRenewalInfo |
| jwsRepresentation for transactions | JWSTransaction | JWSTransaction |

The decoded payload of the jwsRepresentation contains two additional fields: `deviceVerification` and `deviceVerificationNonce`. Use these fields on the device to verify that JWS information belongs to the device. For more information, see deviceVerificationID.

Important

The decoded payloads of jwsRepresentation and JWSTransaction strings contain price or renewalPrice fields specified in *milliunits* of the currency. StoreKit represents the `price` and renewalPrice values in is *units* of the currency. Take care not to confuse these two representations when working with both APIs.

## Topics

### Getting the verification results

case verified(SignedType)

The associated value passed StoreKit automatic verification checks.

case unverified(SignedType, VerificationResult&lt;SignedType>.VerificationError)

The associated value failed StoreKit automatic verification checks.

var payloadValue: SignedType

The verified value of the signed type that StoreKit confirms as verified.

var unsafePayloadValue: SignedType

The associated value of the verification result that StoreKit doesn’t confirm as verified.

enum VerificationError

Error cases for StoreKit JWS verification.

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

var signedData: Data

The transaction data that the signature applies to.

var signatureData: Data

The signature component of the JWS transaction.

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

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

var signature: P256.Signing.ECDSASignature

The signature component of the JSON web signature.

### Getting properties for app transactions

var jwsRepresentation: String

The app transaction signed by the App Store, in JWS Compact Serialization format.

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

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### JWS verification

enum VerificationError

Error cases for StoreKit JWS verification.

