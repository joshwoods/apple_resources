

- StoreKit
- SubscriptionStoreControlStyle
-  Placement 

Associated Type

# Placement

The placement of subscription controls in a subscription store.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
associatedtype Placement : SubscriptionStoreControlPlacement = AutomaticSubscriptionStoreControlPlacement
```

**Required**

## See Also

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

associatedtype Body : View

A view that represents the body of a subscription store control.

**Required**

