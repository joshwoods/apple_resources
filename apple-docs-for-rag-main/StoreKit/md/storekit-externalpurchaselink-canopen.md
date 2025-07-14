

- StoreKit
- ExternalPurchaseLink
-  canOpen 

Type Property

# canOpen

A Boolean value that indicates whether the app can successfully open the configured external purchase link in the current App Store storefront.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static var canOpen: Bool { get async }
```

## Discussion

Use this method if your app configures the SKExternalPurchaseLink property list key.

Check this property, as shown below, to determine whether your app can successfully call open().

```
await ExternalPurchaseLink.canOpen
```

If the result is `true`, configure any user-interface controls that enable people to open the external purchase link. You configure that link in the SKExternalPurchaseLink property list key in the `Info.plist` file. There’s no need to call canOpen again, unless the App Store storefront changes. For more information about the App Store storefront, see Storefront.

This property is `true` if all the following conditions are met:

- The current App Store storefront allows external purchase and the person is eligible to make external purchases.

- Your app configures the com.apple.developer.storekit.external-purchase-link entitlement.

- Your app configures a link for the current App Store storefront in SKExternalPurchaseLink.

Otherwise, this property is `false`.

When this property is `false`, check canMakePayments to determine whether your app can offer in-app purchases using the StoreKit In-App Purchase APIs. For more information, see canMakePayments.

## See Also

### Getting a single external purchase link

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

static func open() async throws

Presents a continuation sheet that enables people to choose whether your app shows its link for external purchases.

