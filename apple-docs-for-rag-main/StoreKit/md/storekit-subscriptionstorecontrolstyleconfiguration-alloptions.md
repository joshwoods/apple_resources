

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  allOptions 

Instance Property

# allOptions

All subscription options in the subscription group.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var allOptions: [Product] { get }
```

## Discussion

The allOptions property is an array that contains all the subscription options in a subscription group. Use the allOptions property to access the subscription options that the options and sections properties may not contain.

For example, use the allOptions property if your control style displays comparisons between available subscription options. A SubscriptionPeriodGroupSet can compare the value of a yearly renewing subscription to a monthly subscription. Because each instance of your control style displays only subscriptions with matching renewal periods, you can’t compute such a comparison using the options property. The allOptions value is always a superset of the options property.

Note

Don’t use the allOptions property to determine the subscription options your control style view displays. Instead, only display the subscription options that the options or sections properties contain.

It’s possible for a subscription store control to display only a subset of the options available within a subscription group. For example, if you use a store content builder to declare the content of a SubscriptionStoreView, the store may create multiple instances of your control with different configuration values. These instances may each display a different subset of the subscripton options.

## See Also

### Getting subscription group properties

var groupDisplayName: String

The localized display name of the subscription group that the subscription store view merchandises.

var autoRenewPreference: Product?

The auto-renewable subscripton product that renews at the next billing cycle.

