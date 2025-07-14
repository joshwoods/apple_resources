

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.PickerOption
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Facilitates accessing product properties on a picker option value.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> T { get }
```

## Discussion

You don’t use this subscript directly. Instead, access the properties of a Product instance directly on a SubscriptionStoreControlStyleConfiguration.PickerOption value.

## See Also

### Dynamic member lookup support

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T?>) -> T?

Facilitates accessing optional subscription properties on a picker option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T>) -> T?

Facilitates accessing subscription properties on a picker option value.

