

- StoreKit
- Ad network attribution
- SKAdNetwork
-  Ad network install-validation keys 

API Collection

# Ad network install-validation keys

Specify key values that validate and associate an app installation with an ad campaign.

## Overview

Ad networks use these keys when calling the product view controller’s loadProduct(withParameters:completionBlock:) method. These keys describe an ad impression in an advertising campaign. The information they contain associates an app installation with an ad campaign. The SKStoreProductParameterITunesItemIdentifier key identifies the advertised app.

Include all the required validation keys in the parameter dictionary for the SKAdNetwork version you’re using.

You also use the values of these keys to generate a signature for the ad impression. For more information, see Generating the signature to validate StoreKit-rendered ads.

## Topics

### Required keys for SKAdNetwork 4 and later

let SKStoreProductParameterAdNetworkSourceIdentifier: String

A four-digit integer that ad networks define to represent the ad campaign.

### Required keys for SKAdNetwork 2 and later

let SKStoreProductParameterAdNetworkVersion: String

The key that represents the version of the ad network API.

let SKStoreProductParameterAdNetworkSourceAppStoreIdentifier: String

The key that represents the App Store ID of the app that displays the ad.

### Required keys

let SKStoreProductParameterAdNetworkIdentifier: String

The key that represents the advertising network’s unique identifier.

let SKStoreProductParameterAdNetworkCampaignIdentifier: String

The key that represents the advertising network’s campaign.

let SKStoreProductParameterAdNetworkTimestamp: String

The key that represents the UNIX time, in milliseconds, of the ad impression.

let SKStoreProductParameterAdNetworkNonce: String

The key that represents a random value to use for added security.

let SKStoreProductParameterAdNetworkAttributionSignature: String

The key that represents the advertising network’s cryptographic signature to use for install validation.

## See Also

### Signing StoreKit-rendered ads

Generating the signature to validate StoreKit-rendered ads

Initiate install validation by displaying a StoreKit-rendered ad with signed parameters.

