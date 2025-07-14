

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  groupDisplayName 

Instance Property

# groupDisplayName

The localized display name of the subscription group that the subscription store view merchandises.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var groupDisplayName: String { get }
```

## Discussion

This property is the same as accessing groupDisplayName on a Product.SubscriptionInfo value. Because all options within a subscription store view belong to the same subscription group, using the groupDisplayName property is more convenient than getting the group display name from an arbitrary subscription option.

## See Also

### Getting subscription group properties

var autoRenewPreference: Product?

The auto-renewable subscripton product that renews at the next billing cycle.

var allOptions: [Product]

All subscription options in the subscription group.

