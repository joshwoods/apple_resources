

- StoreKit
-  SKStoreProductParameterAdNetworkSourceAppStoreIdentifier 

Global Variable

# SKStoreProductParameterAdNetworkSourceAppStoreIdentifier

The key that represents the App Store ID of the app that displays the ad.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
let SKStoreProductParameterAdNetworkSourceAppStoreIdentifier: String
```

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Verifying an install-validation postback

Identifying the parameters in install-validation postbacks

## Discussion

The value for this key is an NSNumber. Provide the App Store item identifier of the app that’s displaying the ad.

During testing, if you’re using a development-signed build to display the ads and not an app from App Store, use `0` as the item identifier.

## See Also

### Required keys for SKAdNetwork 2 and later

let SKStoreProductParameterAdNetworkVersion: String

The key that represents the version of the ad network API.

