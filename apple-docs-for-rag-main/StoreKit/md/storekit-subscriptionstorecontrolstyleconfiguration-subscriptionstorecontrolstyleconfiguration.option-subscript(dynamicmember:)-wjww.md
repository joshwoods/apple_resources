

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.Option
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Facilitates accessing subscription properties on an option value.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> T? { get }
```

## Discussion

You don’t use this subscript directly. Instead, access the properties of Product.SubscriptionInfo directly on a SubscriptionStoreControlStyleConfiguration.Option value. For an example of using a dynamic member lookup, see SubscriptionStoreControlStyleConfiguration.Option.

## See Also

### Looking up dynamic members

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T?>) -> T?

Facilitates accessing optional subscription properties on an option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product, T>) -> T

Facilitates accessing product properties on an option value.

