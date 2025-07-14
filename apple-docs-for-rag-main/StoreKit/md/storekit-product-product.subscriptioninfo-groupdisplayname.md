

- StoreKit
- Product
- Product.SubscriptionInfo
-  groupDisplayName 

Instance Property

# groupDisplayName

The localized name of the subscription group, suitable for display.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
@backDeployed(before: iOS 17.0, macOS 14.0, tvOS 17.0, watchOS 10.0)
var groupDisplayName: String { get }
```

## Discussion

You provide a group display name in App Store Connect when you set up a subscription group. For more information, see Offer auto-renewable subscriptions.

The SubscriptionStoreView uses this value as part of the automatic marketing content if you don’t provide a marketing content view.

Note

When you create a new product in App Store Connect or in a StoreKit configuration file, you can test it before you add a product localization. The groupDisplayName value is an empty string until you add a localization. For more information on localizations, see Add localizations.

## See Also

### Identifying the subscription group

let subscriptionGroupID: String

The subscription group identifier for this subscription.

var groupLevel: Int

The rank of the subscription relative to other subscriptions in the same subscription group.

