

- StoreKit
- VerificationResult
-  payloadValue 

Instance Property

# payloadValue

The verified value of the signed type that StoreKit confirms as verified.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var payloadValue: SignedType { get throws }
```

## Discussion

This property represents the value of a payload in a JSON Web Signature (JWS) value that passed StoreKit verification.

This property throws an error if the JWS value containing the payload doesn’t pass StoreKit’s verification and is therefore *unverified*. To access the payload of an unverified JWS value, get the associated value of the verification result, or use the unsafePayloadValue property.

## See Also

### Getting the verification results

case verified(SignedType)

The associated value passed StoreKit automatic verification checks.

case unverified(SignedType, VerificationResult&lt;SignedType>.VerificationError)

The associated value failed StoreKit automatic verification checks.

var unsafePayloadValue: SignedType

The associated value of the verification result that StoreKit doesn’t confirm as verified.

enum VerificationError

Error cases for StoreKit JWS verification.

