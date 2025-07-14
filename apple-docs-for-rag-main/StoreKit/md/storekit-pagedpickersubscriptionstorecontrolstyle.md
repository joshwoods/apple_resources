

- StoreKit
-  PagedPickerSubscriptionStoreControlStyle 

Structure

# PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct PagedPickerSubscriptionStoreControlStyle
```

## Topics

### Getting the paged picker control style

static var pagedPicker: PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

### Creating the style

init()

Creates a paged picker control style.

### Placing the controls

struct Placement

The placement of paged subscription picker in a subscription store view.

## Relationships

### Conforms To

- Sendable
- SubscriptionStoreControlStyle

## See Also

### Placement types

struct AutomaticSubscriptionStoreControlStyle

The default in-app subscription store control style that resolves its appearance based on the view’s context.

struct ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

struct PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

struct CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact picker control, with a single button to subscribe.

