

- StoreKit
- Product
- Product.SubscriptionInfo
-  subscriptionGroupID 

Instance Property

# subscriptionGroupID

The subscription group identifier for this subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let subscriptionGroupID: String
```

## Discussion

Auto-renewable subscriptions always belong to a subscription group. You create the subscription group identifiers in App Store Connect before you create and add an auto-renewable subscription. For more information about subscription groups, see Offer auto-renewable subscriptions.

## See Also

### Identifying the subscription group

var groupDisplayName: String

The localized name of the subscription group, suitable for display.

var groupLevel: Int

The rank of the subscription relative to other subscriptions in the same subscription group.

