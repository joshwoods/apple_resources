

- StoreKit
-  SubscriptionStoreControlPlacementKey 

Structure

# SubscriptionStoreControlPlacementKey

A placement for a subscription store control in a store view.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SubscriptionStoreControlPlacementKey
```

## Overview

This type represents all available control placements. You typically don’t interact with this type directly. Use it if you create a custom control style that conforms to the SubscriptionStoreControlStyle protocol to restrict the supported placements for your style. By default, a custom control style supports all placements. For more information, see SubscriptionStoreControlPlacement.

## Topics

### Placing subscription store controls

static var bottom: SubscriptionStoreControlPlacementKey

A placement that anchors the subscription controls to the bottom edge of the view.

static var leading: SubscriptionStoreControlPlacementKey

A placement that anchors the subscription controls to the leading edge of the view.

static var scrollView: SubscriptionStoreControlPlacementKey

A placement that locates the subscription controls within the main scroll view of a subscription store view.

static var trailing: SubscriptionStoreControlPlacementKey

A placement that anchors the subscription controls to the trailing edge of the view.

static var bottomBar: SubscriptionStoreControlPlacementKey

A placement that locates the subscription controls in a bar near the bottom of the main scroll view in a subscription store view.

static var buttonsInBottomBar: SubscriptionStoreControlPlacementKey

A hybrid placement that positions subscription controls within the main scroll view, and places auxiliary buttons in the bottom bar.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

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

associatedtype Placement : SubscriptionStoreControlPlacement = AutomaticSubscriptionStoreControlPlacement

The placement of subscription controls in a subscription store.

**Required**

associatedtype Body : View

A view that represents the body of a subscription store control.

**Required**

