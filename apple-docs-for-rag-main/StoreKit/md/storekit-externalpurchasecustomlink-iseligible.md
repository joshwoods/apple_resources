

- StoreKit
- ExternalPurchaseCustomLink
-  isEligible 

Type Property

# isEligible

A Boolean value that indicates at runtime whether the app can use this API to offer custom links for external purchases.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
static var isEligible: Bool { get async }
```

## Discussion

Check this value if your app configures the SKExternalPurchaseCustomLinkRegions property list key. If isEligible is `true`, your app can use the ExternalPurchaseCustomLink API. This value is `true` if all the following conditions are met:

- The current App Store storefront allows custom links for external purchases and the person can make purchases.

- Your app configures the com.apple.developer.storekit.external-purchase-link entitlement.

- Your app configures the current App Store storefront in the SKExternalPurchaseCustomLinkRegions property list key.

If isEligible is `false`, don’t use the ExternalPurchaseCustomLink API. The methods of the ExternalPurchaseCustomLink API throw errors at runtime when isEligible is `false`.

