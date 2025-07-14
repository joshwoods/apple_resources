

- StoreKit
-  SKStoreProductParameterAdNetworkVersion 

Global Variable

# SKStoreProductParameterAdNetworkVersion

The key that represents the version of the ad network API.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+

``` source
let SKStoreProductParameterAdNetworkVersion: String
```

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Identifying the parameters in install-validation postbacks

## Discussion

The value for this key is an NSString. Set this key to version number “`4.0`”, “`3.0`”, “`2.2"`, `“2.1"`, or `"2.0"`. Use the highest available version whenever possible. For version availability, see SKAdNetwork release notes.

Ad networks use this key and the other Ad network install-validation keys when signing ads. For more information, see Generating the signature to validate StoreKit-rendered ads.

## See Also

### Required keys for SKAdNetwork 2 and later

let SKStoreProductParameterAdNetworkSourceAppStoreIdentifier: String

The key that represents the App Store ID of the app that displays the ad.

