

- StoreKit
-  SubscriptionStoreControlStyleConfiguration 

Structure

# SubscriptionStoreControlStyleConfiguration

The properties of a subscription store control that includes the list of auto-renewable subscriptions to merchandise.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SubscriptionStoreControlStyleConfiguration
```

## Overview

When you define a custom subscription store control style by creating a type that conforms to the SubscriptionStoreControlStyle protocol, you implement the makeBody(configuration:) method. That method takes a `SubscriptionStoreControlStyleConfiguration` parameter, which has the information necessary to define the behavior and interactions of a subscription store view’s primary controls.

Decide whether your style supports dividing options into sections.

- If you support sections, use the sections property to preserve the structure and accessory views you declare using SubscriptionOptionSection instances.

- If you don’t support sections, use the options property to have a flattened array of the SubscriptionStoreControlStyleConfiguration.Option values to merchandise.

Provide a control that enables customers to subscribe to each option in either the `options` or `sections` properties.

To hide and sort the subscription options that your view displays, use the initializer of the SubscriptionStoreView. For example, you can initialize the subscription store to contain only the subscription options that upgrade the customer’s current subscription.

Display only the subscription options that appear in either the `options` or `sections` properties. For example, declaring SubscriptionOptionGroup instances can hide certain subscription options from a control. To access information about other subscription options, use the allOptions property.

In cases where a customer is actively subscribed, use autoRenewPreference to get the Product value of the subscription product that renews at the next billing.

## Topics

### Getting subscription options to merchandise

var options: [SubscriptionStoreControlStyleConfiguration.Option]

An array of subscription options for the subscription store view to merchandise.

var sections: [SubscriptionStoreControlStyleConfiguration.Section]

The subscription options to merchandise by sections.

struct Option

Properties of an auto-renewable subscription option to merchandise.

struct PickerOption

The properties of a picker option to use for selecting a subscription.

struct Section

The properties of a section of subscription options within a subscription store control.

struct Icon

A type-erased icon of a subscription option.

### Getting subscription group properties

var groupDisplayName: String

The localized display name of the subscription group that the subscription store view merchandises.

var autoRenewPreference: Product?

The auto-renewable subscripton product that renews at the next billing cycle.

var allOptions: [Product]

All subscription options in the subscription group.

### Getting subscription description visibility

var descriptionVisibility: Visibility

The visibility of product descriptions.

## See Also

### Styling subscription store controls

nonisolated func subscriptionStoreControlStyle(_ style: some SubscriptionStoreControlStyle) -> some View 

Sets the control style for subscription store views within a view.

nonisolated func subscriptionStoreControlStyle&lt;S>(_ style: S, placement: S.Placement) -> some View where S : SubscriptionStoreControlStyle 

Sets the control style and control placement for subscription store views within a view.

protocol SubscriptionStoreControlStyle

A type that specifies the appearance and interaction of controls in the subscription store view instances within the view hierarchy.

protocol SubscriptionStoreControlPlacement

A type that specifies the placement of a subscription control in a subscription store view.

