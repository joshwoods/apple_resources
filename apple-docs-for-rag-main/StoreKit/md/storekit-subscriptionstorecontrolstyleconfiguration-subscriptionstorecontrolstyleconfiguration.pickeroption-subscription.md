

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.PickerOption
-  subscription 

Instance Property

# subscription

The auto-renewable subscription that the picker option represents.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
var subscription: Product { get }
```

## Discussion

SubscriptionStoreControlStyleConfiguration.PickerOption is a dynamic member lookup type, so you don’t need to use this property directly to access the properties of the Product value. Instead, access any properties of Product or Product.SubscriptionInfo directly on the `PickerOption` value.

Important

Don’t use `Product/purchase(confirmIn:options:)` or related purchase methods on this property to initiate a purchase. Use a picker option only for selecting a subscription option, which requires additional confirmation before initiating a purchase.

## See Also

### Getting properties of the subscription picker option

var activeOffer: Product.SubscriptionOffer?

let isSelected: Bool

A Boolean value that indicates whether the picker option is in a selected state.

var icon: SubscriptionStoreControlStyleConfiguration.Icon?

The subscription option’s icon.

var id: Product.ID

