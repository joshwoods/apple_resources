

- StoreKit
-  SKStoreProductParameterAdNetworkCampaignIdentifier 

Global Variable

# SKStoreProductParameterAdNetworkCampaignIdentifier

The key that represents the advertising network’s campaign.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+

``` source
let SKStoreProductParameterAdNetworkCampaignIdentifier: String
```

## Mentioned in 

Combining parameters to generate a signature for SKAdNetwork 1

Identifying the parameters in install-validation postbacks

Generating the signature to validate StoreKit-rendered ads

## Discussion

The value for this key is an NSNumber. Ad networks determine their own campaign identifiers, which must be an integer `>=1` and `SKStoreProductParameterAdNetworkSourceIdentifier instead of this value to generate version 4 and later signatures.

## See Also

### Required keys

let SKStoreProductParameterAdNetworkIdentifier: String

The key that represents the advertising network’s unique identifier.

let SKStoreProductParameterAdNetworkTimestamp: String

The key that represents the UNIX time, in milliseconds, of the ad impression.

let SKStoreProductParameterAdNetworkNonce: String

The key that represents a random value to use for added security.

let SKStoreProductParameterAdNetworkAttributionSignature: String

The key that represents the advertising network’s cryptographic signature to use for install validation.

