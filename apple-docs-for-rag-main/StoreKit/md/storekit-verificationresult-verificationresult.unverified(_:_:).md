

- StoreKit
- VerificationResult
-  VerificationResult.unverified(\_:\_:) 

Case

# VerificationResult.unverified(\_:\_:)

The associated value failed StoreKit automatic verification checks.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case unverified(SignedType, VerificationResult.VerificationError)
```

## Discussion

The first associated value in this case is the App Store-signed value. The second associated value provides the reason why the verification failed.

## See Also

### Getting the verification results

case verified(SignedType)

The associated value passed StoreKit automatic verification checks.

var payloadValue: SignedType

The verified value of the signed type that StoreKit confirms as verified.

var unsafePayloadValue: SignedType

The associated value of the verification result that StoreKit doesn’t confirm as verified.

enum VerificationError

Error cases for StoreKit JWS verification.

