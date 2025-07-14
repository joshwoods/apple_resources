

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  SubscriptionStoreControlStyleConfiguration.PickerOption 

Structure

# SubscriptionStoreControlStyleConfiguration.PickerOption

The properties of a picker option to use for selecting a subscription.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@dynamicMemberLookup
struct PickerOption
```

## Overview

You use `SubscriptionStoreControlStyleConfiguration.PickerOption` very similarly to SubscriptionStoreControlStyleConfiguration.Option. The key differences are:

- The picker option represents a subscription option within the scope of an element of a picker control, where you can merchandise a standard option using any kind of control.

- Instead of getting an option from a SubscriptionStoreControlStyleConfiguration, you get a picker option when you create a SubscriptionStorePicker.

- Instead of providing a subscribe() method, the picker option provides an isSelected property to get the selection state.

The key difference is a `SubscriptionStoreControlStyleConfiguration.Option` provides a method to subscribe, and a `SubscriptionStoreControlStyleConfiguration.PickerOption` indicates the current selection state within a SubscriptionStorePicker.

SubscriptionStoreControlStyleConfiguration.PickerOption is a dynamic member lookup type, so you don’t need to use subscription directly to access the properties of the `Product` value. Instead, access any properties of `Product` or Product.SubscriptionInfo directly on the `PickerOption` value.

## Topics

### Getting properties of the subscription picker option

var subscription: Product

The auto-renewable subscription that the picker option represents.

var activeOffer: Product.SubscriptionOffer?

let isSelected: Bool

A Boolean value that indicates whether the picker option is in a selected state.

var icon: SubscriptionStoreControlStyleConfiguration.Icon?

The subscription option’s icon.

var id: Product.ID

### Dynamic member lookup support

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T?>) -> T?

Facilitates accessing optional subscription properties on a picker option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product.SubscriptionInfo, T>) -> T?

Facilitates accessing subscription properties on a picker option value.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Product, T>) -> T

Facilitates accessing product properties on a picker option value.

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

struct Option

Properties of an auto-renewable subscription option to merchandise.

struct Section

The properties of a section of subscription options within a subscription store control.

struct Icon

A type-erased icon of a subscription option.

