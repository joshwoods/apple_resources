

- StoreKit
- SubscriptionStoreControlStyle
-  buttons 

Type Property

# buttons

A subscription store control style that displays a subscribe button for each subscription plan.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
static var buttons: ButtonsSubscriptionStoreControlStyle { get }
```

## Discussion

You can also use subscriptionStoreControlStyle(_:) with buttons as the parameter to construct this style.

## See Also

### Getting built-in subscription store control styles

static var automatic: AutomaticSubscriptionStoreControlStyle

A subscription store control style that resolves its appearance automatically, based on the current context.

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

