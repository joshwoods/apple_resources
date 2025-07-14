

- StoreKit
-  SKStoreProductParameterAdNetworkIdentifier 

Global Variable

# SKStoreProductParameterAdNetworkIdentifier

The key that represents the advertising network’s unique identifier.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+

``` source
let SKStoreProductParameterAdNetworkIdentifier: String
```

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Identifying the parameters in install-validation postbacks

Combining parameters to generate a signature for SKAdNetwork 1

## Discussion

The value for this key is an NSString.

Ad networks obtain an ad network identifier during registration. Ad networks are responsible for sharing their ad network IDs with participating app developers. Apps that display ads and need to initiate the app install validation process must include the ad network ID in their `Info.plist`. For more information see Registering an ad network and `Configuring Apps`.

## See Also

### Required keys

let SKStoreProductParameterAdNetworkCampaignIdentifier: String

The key that represents the advertising network’s campaign.

let SKStoreProductParameterAdNetworkTimestamp: String

The key that represents the UNIX time, in milliseconds, of the ad impression.

let SKStoreProductParameterAdNetworkNonce: String

The key that represents a random value to use for added security.

let SKStoreProductParameterAdNetworkAttributionSignature: String

The key that represents the advertising network’s cryptographic signature to use for install validation.

