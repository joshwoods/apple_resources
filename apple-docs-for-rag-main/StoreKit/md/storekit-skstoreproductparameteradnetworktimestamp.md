

- StoreKit
-  SKStoreProductParameterAdNetworkTimestamp 

Global Variable

# SKStoreProductParameterAdNetworkTimestamp

The key that represents the UNIX time, in milliseconds, of the ad impression.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+

``` source
let SKStoreProductParameterAdNetworkTimestamp: String
```

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Combining parameters to generate a signature for SKAdNetwork 1

## Discussion

The value for this key is an NSNumber. Ad networks generate the timestamp, represented as UNIX time in milliseconds, at the time you’re preparing to serve the ad.

## See Also

### Required keys

let SKStoreProductParameterAdNetworkIdentifier: String

The key that represents the advertising network’s unique identifier.

let SKStoreProductParameterAdNetworkCampaignIdentifier: String

The key that represents the advertising network’s campaign.

let SKStoreProductParameterAdNetworkNonce: String

The key that represents a random value to use for added security.

let SKStoreProductParameterAdNetworkAttributionSignature: String

The key that represents the advertising network’s cryptographic signature to use for install validation.

