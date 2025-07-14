

- StoreKit
-  SKStoreProductParameterAdNetworkNonce 

Global Variable

# SKStoreProductParameterAdNetworkNonce

The key that represents a random value to use for added security.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+

``` source
let SKStoreProductParameterAdNetworkNonce: String
```

## Mentioned in 

Combining parameters to generate a signature for SKAdNetwork 1

Generating the signature to validate StoreKit-rendered ads

Combining parameters to generate a signature for SKAdNetwork 2

Combining parameters to generate signatures for SKAdNetwork 2.2 and 3

## Discussion

The value for this key is an NSUUID. Ad networks generate a random value for this key at the time of the ad impression.

Important

When you generate the signature value (SKStoreProductParameterAdNetworkAttributionSignature), you must sign the nonce as an all-lowercase UUID string representation.

## See Also

### Required keys

let SKStoreProductParameterAdNetworkIdentifier: String

The key that represents the advertising network’s unique identifier.

let SKStoreProductParameterAdNetworkCampaignIdentifier: String

The key that represents the advertising network’s campaign.

let SKStoreProductParameterAdNetworkTimestamp: String

The key that represents the UNIX time, in milliseconds, of the ad impression.

let SKStoreProductParameterAdNetworkAttributionSignature: String

The key that represents the advertising network’s cryptographic signature to use for install validation.

