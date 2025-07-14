

- StoreKit
- AppStore
-  deviceVerificationID 

Type Property

# deviceVerificationID

The device verification identifier to use to verify whether signed information is valid for the current device.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var deviceVerificationID: UUID? { get }
```

## Discussion

Use this property to verify whether an App Store-signed JSON Web Signature (JWS) is valid for the current device. The JWS may be one of the following:

- A jwsRepresentation representing a signed transaction

- A jwsRepresentation representing a signed subscription renewal information

- A jwsRepresentation representing a signed app transaction.

To verify that the JWS is valid for the current device, follow these steps:

1.  Append the lowercased UUID string representation of this property, deviceVerificationID, after the lowercased UUID string representation of the device verification nonce. For a transaction, the nonce is deviceVerificationNonce. For subscription renewal information, the nonce is deviceVerificationNonce. For an app transaction, the nonce is deviceVerificationNonce.

2.  Compute the SHA-384 hash of the appended UUID strings.

3.  Verify that the SHA-384 digest is equal to the device verification property. For a transaction, the device verification property is deviceVerification. For subscription renewal information, the device verification property is deviceVerification. For an app transaction, the device verifcation property is deviceVerification.

