

- StoreKit
-  SKStoreProductParameterAdNetworkSourceIdentifier 

Global Variable

# SKStoreProductParameterAdNetworkSourceIdentifier

A four-digit integer that ad networks define to represent the ad campaign.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+tvOS 16.1+

``` source
let SKStoreProductParameterAdNetworkSourceIdentifier: String
```

## Mentioned in 

SKAdNetwork 4 release notes

Generating the signature to validate StoreKit-rendered ads

Identifying the parameters in install-validation postbacks

## Discussion

This key is available for ad impressions that use SKAdNetwork 4 and later. The SKStoreProductParameterAdNetworkSourceIdentifier, also known as the *hierarchical source identifier*, replaces and extends the campaign identifier value, SKStoreProductParameterAdNetworkCampaignIdentifier.

Ad networks and developers define the meaning of the hierarchical source identifier. This string represents an integer of up to four digits. You can encode information about your advertisement in each set of digits; you may receive two, three, or all four digits of the sourceIdentifier in the first winning postback, depending on the ad impression’s postback data tier. For more information about the value you may get in the postback, see Receiving postbacks in multiple conversion windows.

