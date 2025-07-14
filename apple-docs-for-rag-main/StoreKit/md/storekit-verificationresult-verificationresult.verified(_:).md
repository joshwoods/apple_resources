

- StoreKit
- VerificationResult
-  VerificationResult.verified(\_:) 

Case

# VerificationResult.verified(\_:)

The associated value passed StoreKit automatic verification checks.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case verified(SignedType)
```

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

The associated value in this case is the App Store-signed value.

## See Also

### Getting the verification results

case unverified(SignedType, VerificationResult&lt;SignedType>.VerificationError)

The associated value failed StoreKit automatic verification checks.

var payloadValue: SignedType

The verified value of the signed type that StoreKit confirms as verified.

var unsafePayloadValue: SignedType

The associated value of the verification result that StoreKit doesn’t confirm as verified.

enum VerificationError

Error cases for StoreKit JWS verification.

