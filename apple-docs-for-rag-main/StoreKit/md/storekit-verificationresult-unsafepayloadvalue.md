

- StoreKit
- VerificationResult
-  unsafePayloadValue 

Instance Property

# unsafePayloadValue

The associated value of the verification result that StoreKit doesn’t confirm as verified.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var unsafePayloadValue: SignedType { get }
```

## Discussion

This property represents the value of a payload in a JSON Web Signature (JWS) value that’s not confirmed to have passed StoreKit verification.

Use the unsafePayloadValue for debugging purposes or other situations where the integrity of the data is unimportant. This property ignores any verification errors. To get a payload that passed verification, or to check for verification errors, use the payloadValue property instead.

Important

Don’t trust the integrity of the values you receive from the unsafePayloadValue property. This property contains data regardless of the verification result, and contains data even if StoreKit’s verification fails.

To determine if the JWS value fails verification, perform a verification on the jwsRepresentation property for subscription renewal information, the jwsRepresentation property for transactions, or the jwsRepresentation property for app transactions.

## See Also

### Getting the verification results

case verified(SignedType)

The associated value passed StoreKit automatic verification checks.

case unverified(SignedType, VerificationResult&lt;SignedType>.VerificationError)

The associated value failed StoreKit automatic verification checks.

var payloadValue: SignedType

The verified value of the signed type that StoreKit confirms as verified.

enum VerificationError

Error cases for StoreKit JWS verification.

