

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.PickerOption
-  icon 

Instance Property

# icon

The subscription option’s icon.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
var icon: SubscriptionStoreControlStyleConfiguration.Icon? { get }
```

## Discussion

Use this property to access the icon you configure for a subscription option using the subscriptionStoreControlIcon(icon:) view modifier.

## See Also

### Getting properties of the subscription picker option

var subscription: Product

The auto-renewable subscription that the picker option represents.

var activeOffer: Product.SubscriptionOffer?

let isSelected: Bool

A Boolean value that indicates whether the picker option is in a selected state.

var id: Product.ID

