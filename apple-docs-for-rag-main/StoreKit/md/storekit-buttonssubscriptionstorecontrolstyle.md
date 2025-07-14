

- StoreKit
-  ButtonsSubscriptionStoreControlStyle 

Structure

# ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct ButtonsSubscriptionStoreControlStyle
```

## Topics

### Getting the button subscription store style

static var buttons: ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

### Creating the style

init()

Creates a button subscription store control style.

## Relationships

### Conforms To

- Sendable
- SubscriptionStoreControlStyle

## See Also

### Placement types

struct AutomaticSubscriptionStoreControlStyle

The default in-app subscription store control style that resolves its appearance based on the view’s context.

struct PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

struct CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact picker control, with a single button to subscribe.

struct PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

