

- StoreKit
- SubscriptionStoreControlStyle
-  pagedPicker 

Type Property

# pagedPicker

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
static var pagedPicker: PagedPickerSubscriptionStoreControlStyle { get }
```

## See Also

### Getting built-in subscription store control styles

static var automatic: AutomaticSubscriptionStoreControlStyle

A subscription store control style that resolves its appearance automatically, based on the current context.

static var buttons: ButtonsSubscriptionStoreControlStyle

A subscription store control style that displays a subscribe button for each subscription plan.

static var picker: PickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a picker control, with a single button to subscribe.

static var prominentPicker: ProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent picker control, with a single button to subscribe.

static var pagedProminentPicker: PagedProminentPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a prominent paged picker control, with a single button to subscribe.

static var compactPicker: CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact control, with a single button to subscribe.

