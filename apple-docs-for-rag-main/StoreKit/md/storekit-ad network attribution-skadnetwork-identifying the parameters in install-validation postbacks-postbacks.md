

- StoreKit
- Ad network attribution
- SKAdNetwork
-  Identifying the parameters in install-validation postbacks 

Article

# Identifying the parameters in install-validation postbacks

Learn about the postback parameters in all SKAdNetwork versions.

## Overview

The following list describes all the possible parameters you may get in a postback, and their version availability. To verify that Apple signed the postback, see Verifying an install-validation postback.

`version`  
Version 2 and later. The SKAdNetwork version that matches SKStoreProductParameterAdNetworkVersion or version. For more information about versions, see SKAdNetwork release notes.

`ad-network-id`  
Version 1 and later. Your ad network ID, which matches the value you provide for SKStoreProductParameterAdNetworkIdentifier or adNetworkIdentifier.

`attribution-signature`  
Version 2 and later. Apple’s attribution signature that you verify.

`app-id`  
Version 1 and later. The App Store app ID of the advertised app.

`source-identifier`  
Version 4 and later. The hierarchical source identifier that replaces the `campaign-id`. This string represents two, three, or four digits of the original value the ad network supplies in SKStoreProductParameterAdNetworkSourceIdentifier or sourceIdentifier.

`campaign-id`  
Versions 1–3. The campaign identifer you provide when displaying the ad, which matches SKStoreProductParameterAdNetworkCampaignIdentifier or adCampaignIdentifier. Version 4 and later ads use `source-identifer` instead.

`source-app-id`  
Version 2 and later. The App Store app ID of the app that displays the ad. The `source-app-id` value matches SKStoreProductParameterAdNetworkSourceAppStoreIdentifier or sourceAppStoreItemIdentifier.

Note: The `source-app-id` only appears in the postback if providing the parameter meets Apple’s privacy threshold.

`source-domain`  
Version 4 and later, for web ads only. For more information, see SKAdNetwork for Web Ads.

`conversion-value`  
Version 2 and later. An unsigned 6-bit value that the installed app sets by calling a method to update the conversion value, such as updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:). The `conversion-value` only appears in the postback if the installed app provides it, and if providing the parameter meets Apple’s privacy threshold.

Note: The signature doesn’t include the `conversion-value`. Postbacks may contain either `conversion-value` or `coarse-conversion-value`, not both.

`coarse-conversion-value`  
Version 4 and later. Possible values are the strings `"low"`, `"medium"`, and `"high"`. The installed app sets this value by calling a method to update conversion values, such as updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:).

Note: The signature doesn’t include the `coarse-conversion-value`. Postbacks may contain either `conversion-value` or `coarse-conversion-value`, not both.

`did-win`  
Version 3 and later. A Boolean value that’s `true` if the ad network wins the attribution, and `false` if the postback represents a qualifying ad impression that doesn’t win the attribution.

`fidelity-type`  
Version 2.2 and later. A value of `0` indicates a view-through ad presentation; a value of `1` indicates a StoreKit-rendered ad or an SKAdNetwork-attributed web ad.

`postback-sequence-index`  
Version 4 and later. The possible integer values of `0`, `1`, and `2` signify the order of postbacks that result from the three conversion windows. For more information, see Receiving postbacks in multiple conversion windows.

`redownload`  
Version 2 and later. A Boolean value of `true` indicates that a device with the customer’s Apple ID previously installed the app.

`transaction-id`  
Version 1 and later. A unique value for this validation; use it to deduplicate install-validation postbacks.

To ensure crowd anonymity, Apple assigns a postback data tier to app downloads. The postback data tier determines whether certain parameters appear in the postback, as well as the number of digits in the hierarchical source identifer. The following postback parameters are subject to the postback data tier:

- `source-identifier` (affects the number of digits the postback returns)

- `coarse-conversion-value`

- `conversion-value`

- `source-app-id`

- `source-domain`

For more information about receiving postbacks, see Receiving postbacks in multiple conversion windows.

## See Also

### Verifying postbacks

Verifying an install-validation postback

Ensure the validity of a postback you receive after an ad conversion by verifying its cryptographic signature.

