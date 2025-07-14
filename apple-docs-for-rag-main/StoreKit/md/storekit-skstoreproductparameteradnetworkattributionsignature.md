

- StoreKit
-  SKStoreProductParameterAdNetworkAttributionSignature 

Global Variable

# SKStoreProductParameterAdNetworkAttributionSignature

The key that represents the advertising network’s cryptographic signature to use for install validation.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+

``` source
let SKStoreProductParameterAdNetworkAttributionSignature: String
```

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Signing and providing ads

## Discussion

The value for this key is an NSString. The ad network creates the cryptographic signature, used to sign ads. For instructions on generating this value, see Generating the signature to validate StoreKit-rendered ads.

## See Also

### Required keys

let SKStoreProductParameterAdNetworkIdentifier: String

The key that represents the advertising network’s unique identifier.

let SKStoreProductParameterAdNetworkCampaignIdentifier: String

The key that represents the advertising network’s campaign.

let SKStoreProductParameterAdNetworkTimestamp: String

The key that represents the UNIX time, in milliseconds, of the ad impression.

let SKStoreProductParameterAdNetworkNonce: String

The key that represents a random value to use for added security.

