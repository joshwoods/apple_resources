

- StoreKit
- SubscriptionStoreControlStyle
-  SubscriptionStoreControlStyle.Configuration 

Type Alias

# SubscriptionStoreControlStyle.Configuration

The properties of a subscription store control that includes the list of auto-renewable subscriptions to merchandise.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Configuration = SubscriptionStoreControlStyleConfiguration
```

## See Also

### Creating custom subscription store control styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a subscription store control.

**Required**

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

