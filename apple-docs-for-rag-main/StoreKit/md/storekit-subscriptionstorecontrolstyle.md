

- StoreKit
-  SubscriptionStoreControlStyle 

Protocol

# SubscriptionStoreControlStyle

A type that specifies the appearance and interaction of controls in the subscription store view instances within the view hierarchy.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
protocol SubscriptionStoreControlStyle
```

## Overview

Use the subscriptionStoreControlStyle(_:) view modifier to configure the subscription store control style for a view hierarchy.

```
SubscriptionStoreView(groupID: "SAMPLE")
    .subscriptionStoreControlStyle(.prominentPicker)
```

You can also configure the control placement using the subscriptionStoreControlStyle(_:placement:) view modifier.

### Create custom styles

To create a custom style, declare a type that conforms to the `SubscriptionStoreControlStyle` protocol and implement the required makeBody(configuration:) method. For example, you can define a style that adds price comparison captions to buttons.

```
struct PriceComparisonButtonsSubscriptionStoreControlStyle: SubscriptionStoreControlStyle {

    func makeBody(configuration: Configuration) -> some View {
        // Return a view displaying a captioned button for each option.
    }
}
```

Inside the method, use the `configuration` parameter, which is a SubscriptionStoreControlStyleConfiguration value, to get the properties of the control, such as the subscriptions to merchandise. For examples that show constructing a view from the configuration value, see makeBody(configuration:).

The subscription store control style protocol has a Placement associated type, which represents the placements that the style supports. To optionally restrict the placements your custom style supports, explicitly declare a type alias named `Placement`. For more information about restricting placements, see SubscriptionStoreControlPlacement. If you don’t declare the type alias, your custom style automatically uses the AutomaticSubscriptionStoreControlPlacement as its Placement associated type.

The following code example declares a `Placement` type alias:

```
struct PriceComparisonButtonsSubscriptionStoreControlStyle: SubscriptionStoreControlStyle {

    // Support the same placements as the standard buttons style.
    typealias Placement = ButtonsSubscriptionStoreControlStyle.Placement

    func makeBody(configuration: Configuration) -> some View {
        // Return a view displaying a captioned button for each option.
    }
}
```

To provide easy access to the new style, declare a corresponding static variable in an extension to `SubscriptionStoreControlStyle`.

```
extension SubscriptionStoreControlStyle where Self == 
PriceComparisonButtonsSubscriptionStoreControlStyle {
    static var priceComparisonButtons: Self { Self() }
}
```

Then, use your custom style as follows:

```
SubscriptionStoreView(groupID: "SAMPLE")
    .subscriptionStoreControlStyle(.priceComparisonButtons)
```

## Topics

### Getting built-in subscription store control styles

static var automatic: AutomaticSubscriptionStoreControlStyle

A subscription store control style that resolves its appearance automatically, based on the current context.

static var buttons: ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

static var picker: PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

static var prominentPicker: ProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent picker control, with a single button to subscribe.

static var pagedPicker: PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

static var pagedProminentPicker: PagedProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent paged picker control, with a single button to subscribe.

static var compactPicker: CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact control, with a single button to subscribe.

### Creating custom subscription store control styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a subscription store control.

**Required**

typealias Configuration

The properties of a subscription store control that includes the list of auto-renewable subscriptions to merchandise.

typealias SubscribeButton

A button for subscribing to an in-app subscription.

typealias SubscriptionPicker

A composite control for selecting a subscription option and confirming the subscription.

typealias SubscriptionPickerOption

A subscription option within a subscription picker control.

struct SubscriptionStoreControlPlacementKey

A placement for a subscription store control in a store view.

associatedtype Placement : SubscriptionStoreControlPlacement = AutomaticSubscriptionStoreControlPlacement

The placement of subscription controls in a subscription store.

**Required**

associatedtype Body : View

A view that represents the body of a subscription store control.

**Required**

### Supporting types

struct AutomaticSubscriptionStoreControlStyle

The default in-app subscription store control style that resolves its appearance based on the view’s context.

struct ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

struct PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

struct ProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent picker control, with a single button to subscribe.

struct CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact picker control, with a single button to subscribe.

struct PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

struct PagedProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged prominent picker control, with a single button to subscribe.

struct AutomaticSubscriptionStoreControlPlacement

A system-defined placement for a subscription store view.

## Relationships

### Conforming Types

- AutomaticSubscriptionStoreControlStyle
- ButtonsSubscriptionStoreControlStyle
- CompactPickerSubscriptionStoreControlStyle
- PagedPickerSubscriptionStoreControlStyle
- PagedProminentPickerSubscriptionStoreControlStyle
- PickerSubscriptionStoreControlStyle
- ProminentPickerSubscriptionStoreControlStyle

## See Also

### Styling subscription store controls

nonisolated func subscriptionStoreControlStyle(_ style: some SubscriptionStoreControlStyle) -> some View 

Sets the control style for subscription store views within a view.

nonisolated func subscriptionStoreControlStyle&lt;S>(_ style: S, placement: S.Placement) -> some View where S : SubscriptionStoreControlStyle 

Sets the control style and control placement for subscription store views within a view.

struct SubscriptionStoreControlStyleConfiguration

The properties of a subscription store control that includes the list of auto-renewable subscriptions to merchandise.

protocol SubscriptionStoreControlPlacement

A type that specifies the placement of a subscription control in a subscription store view.

