

- StoreKit
- Product
- Product.SubscriptionInfo
-  groupLevel 

Instance Property

# groupLevel

The rank of the subscription relative to other subscriptions in the same subscription group.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
@backDeployed(before: iOS 17.0, macOS 14.0, tvOS 17.0, watchOS 10.0)
var groupLevel: Int { get }
```

## Discussion

If you offer multiple auto-renewable subscriptions with different price tiers, you can assign each to a level in App Store Connect. Ranking your subscriptions determines the upgrade, downgrade, and crossgrade paths available.

Subscriptions with the highest level of service within a subscription group have a groupLevel value of `1`. Subscriptions with lower levels of service or content have groupLevel values of `2` or greater. For example, when comparing two subscriptions, moving from a subscription with a groupLevel of `2` to a subscription with a groupLevel of `1` represents an upgrade.

For more information on ranking, see Ranking subscriptions within the group. For information on assigning subscription levels in App Store Connect, see Assign subscription levels.

Note

On systems earlier than iOS 17, macOS 14, tvOS 17, and watchOS 10, this property returns a sentinel value of `0` when you test your app using StoreKit Testing in Xcode or if there’s an unexpected server error.

## See Also

### Identifying the subscription group

let subscriptionGroupID: String

The subscription group identifier for this subscription.

var groupDisplayName: String

The localized name of the subscription group, suitable for display.

