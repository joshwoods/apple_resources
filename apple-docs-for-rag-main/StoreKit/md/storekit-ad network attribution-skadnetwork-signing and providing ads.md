

- StoreKit
- Ad network attribution
- SKAdNetwork
-  Signing and providing ads 

Article

# Signing and providing ads

Advertise apps by signing and providing StoreKit-rendered ads, view-through ads, or attributable web ads.

## Overview

SKAdNetwork supports several ways for ad networks to provide ads:

- StoreKit-rendered ads, where StoreKit displays an App Store product page as the ad impression

- View-through ads, where the ad network presents an ad in any format and reports the ad impression using the SKAdNetwork API

- Attributable web ads, where the ad network presents an ad on a Safari web page using the SKAdNetwork for Web Ads API

To differentiate StoreKit-rendered ads from view-through ads, SKAdNetwork defines a `fidelity-type` parameter, which you include in the ad signature, and receive in the install-validation postback. Use a `fidelity-type` value of `1` for StoreKit-rendered ads and attributable web ads, and `0` for view-through ads. The following table compares the ad presentation options:

| Ad presentation option | Description | Fidelity type | Availability |
|----|----|----|----|
| StoreKit-rendered ads | App Store product page that StoreKit renders | `1` | All SKAdNetwork versions |
| View-through ads | Custom, from the ad network | `0` | SKAdNetwork 2.2 and later |
| Attributable web ads (SKAdNetwork for Web Ads) | Custom, from the ad network | `1` | SKAdNetwork 4 and later |

For more information about availability and versions, see SKAdNetwork release notes.

The `fidelity-type` can affect which ad receives attribution when the user experiences multiple ad impressions. For more information about how `fidelity-type` and the time of the ad impression affect attributions, see Receiving ad attributions and postbacks.

Ad networks must cryptographically sign the ads. The signature contains information that includes a campaign identifier. If ads result in conversions, ad networks receive an install-validation postback that includes the campaign identifier. For more information about the postback, see Verifying an install-validation postback.

### Provide a StoreKit-rendered ad

Follow these steps to display a StoreKit-rendered ad in your app:

1.  Set Ad network install-validation keys with values that represent the ad impression.

2.  On the ad network’s server, generate the signature using those key values. Then, set the SKStoreProductParameterAdNetworkAttributionSignature key with the signature value. For information about generating the signature, see Generating the signature to validate StoreKit-rendered ads.

3.  Call loadProduct(withParameters:completionBlock:) using your ad network install-validation keys to load the ad.

4.  Present the ad in your app according to your app’s design. You can use either an SKOverlay or an SKStoreProductViewController to display a StoreKit-rendered ad. The `fidelity-type` value of a StoreKit-rendered ad is `1` in either case.

### Provide a view-through ad

Follow these steps to provide a view-through ad:

1.  Create an SKAdImpression instance and set its properties to represent the ad impression.

2.  On the ad network’s server, generate the signature based on those properties. Then set the signature property in the SKAdImpression instance to the generated signature. For more information, see Generating the signature to validate view-through ads.

3.  Call startImpression(_:completionHandler:) and then present your custom ad to the user according to your app’s design.

4.  Call endImpression(_:completionHandler:) when you finish presenting the ad.

### Provide an attributable web ad

Ad networks can sign attributable ads that websites can display in Safari. For more information, see SKAdNetwork for Web Ads.

## See Also

### Essentials

Receiving ad attributions and postbacks

Learn about timeframes and priorities for ad impressions that result in ad attributions, and how additional impressions qualify for postbacks.

Receiving postbacks in multiple conversion windows

Learn about the data that postbacks may contain in each conversion window.

SKAdNetwork release notes

Learn about the features in each SKAdNetwork version.

