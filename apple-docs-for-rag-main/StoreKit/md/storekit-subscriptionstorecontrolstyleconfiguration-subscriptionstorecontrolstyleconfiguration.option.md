

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  SubscriptionStoreControlStyleConfiguration.Option 

Structure

# SubscriptionStoreControlStyleConfiguration.Option

Properties of an auto-renewable subscription option to merchandise.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@dynamicMemberLookup
struct Option
```

## Overview

You use `SubscriptionStoreControlStyleConfiguration.Option` very similarly to Product values, with some important differences:

- The `offer` property indicates the offer that applies to the purchase. Display the terms of the `offer`, and ignore offer properties on Product.SubscriptionInfo, such as introductoryOffer.

- If the `offer` is `nil`, no offer applies to the purchase.

- Call the subscribe() method when a customer activates a control to subscribe to a subscription option, instead of methods on Product, such as `Product/purchase(confirmIn:options:)`.

- Access the decorative icon using the icon property.

`SubscriptionStoreControlStyleConfiguration.Option` is a dynamic member lookup type, so you don’t need to use subscription directly to access the properties of the `Product` value. Instead, access the properties of `Product` or Product.SubscriptionInfo directly on the `Option` value. In the example below, the displayName property is available on `Option` to use as the button label:

```
struct DisplayNameButtonsControlStyle: SubscriptionStoreControlStyle {

    func makeBody(configuration: Configuration) -> some View {
        ForEach(configuration.options) { option in
            Button(option.displayName, action: option.subscribe)
        }
    }
}
```

## Topics

### Getting the subscription product and offer

var subscription: Product

The auto-renewable subscription to merchandise.

var id: Product.ID

The product ID of the auto-renewable subscription.

var activeOffer: Product.SubscriptionOffer?

The subscription offer the customer is eligible for, and that applies to the subscription option.

### Getting the icon

var icon: SubscriptionStoreControlStyleConfiguration.Icon?

The subscription option’s icon.

### Purchasing a subscription option

func subscribe()

Initiates a purchase when a customer activates a control to subscribe to the option.

### Looking up dynamic members

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T?>) -> T?

Facilitates accessing optional subscription properties on an option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T>) -> T?

Facilitates accessing subscription properties on an option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product, T>) -> T

Facilitates accessing product properties on an option value.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable

## See Also

### Getting subscription options to merchandise

var options: [SubscriptionStoreControlStyleConfiguration.Option]

An array of subscription options for the subscription store view to merchandise.

var sections: [SubscriptionStoreControlStyleConfiguration.Section]

The subscription options to merchandise by sections.

struct PickerOption

The properties of a picker option to use for selecting a subscription.

struct Section

The properties of a section of subscription options within a subscription store control.

struct Icon

A type-erased icon of a subscription option.

