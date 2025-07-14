

- StoreKit
- SKAdImpression
-  signature 

Instance Property

# signature

The advertising network’s cryptographic signature for the ad impression.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var signature: String { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

Signing and providing ads

## Discussion

The ad network creates a cryptographic signature that it uses to sign ads. For instructions on generating this value, see Generating the signature to validate view-through ads.

