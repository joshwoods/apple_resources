

- StoreKit
-  SubscriptionStorePickerOption 

Structure

# SubscriptionStorePickerOption

A subscription option within a subscription picker control.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct SubscriptionStorePickerOption where Label : View
```

## Topics

### Creating a subscription picker option

init(SubscriptionStoreControlStyleConfiguration.Option)

init(SubscriptionStoreControlStyleConfiguration.PickerOption)

init(SubscriptionStoreControlStyleConfiguration.Option, label: (SubscriptionStoreControlStyleConfiguration.PickerOption) -> Label)

### Supporting types

struct AutomaticSubscriptionStorePickerOptionLabel

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Creating custom subscription store control styles

struct SubscriptionStoreButton

A button for subscribing to an in-app subscription with a localized label and optional caption.

struct SubscriptionStorePicker

A composite control with a picker for selecting a subscription option and a button for confirming the subscription.

