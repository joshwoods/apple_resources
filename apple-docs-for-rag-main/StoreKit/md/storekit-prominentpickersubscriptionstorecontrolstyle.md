

- StoreKit
-  ProminentPickerSubscriptionStoreControlStyle 

Structure

# ProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent picker control, with a single button to subscribe.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
@MainActor @preconcurrency
struct ProminentPickerSubscriptionStoreControlStyle
```

## Topics

### Getting the prominent picker control style

static var pagedProminentPicker: PagedProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent paged picker control, with a single button to subscribe.

### Creating the style

init()

Creates a prominent picker subscription store control style.

### Placing the controls

associatedtype Placement : SubscriptionStoreControlPlacement = AutomaticSubscriptionStoreControlPlacement

The placement of subscription controls in a subscription store.

**Required**

## Relationships

### Conforms To

- Sendable
- SubscriptionStoreControlStyle

## See Also

### Supporting types

struct AutomaticSubscriptionStoreControlStyle

The default in-app subscription store control style that resolves its appearance based on the view’s context.

struct ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

struct PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

struct CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact picker control, with a single button to subscribe.

struct PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

struct PagedProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged prominent picker control, with a single button to subscribe.

struct AutomaticSubscriptionStoreControlPlacement

A system-defined placement for a subscription store view.

