

- StoreKit
-  AutomaticSubscriptionStoreControlPlacement 

Structure

# AutomaticSubscriptionStoreControlPlacement

A system-defined placement for a subscription store view.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AutomaticSubscriptionStoreControlPlacement
```

## Overview

You typically don’t use this type directly, except when you implement a custom control style. By default, a custom control style supports all placements. For more information, see the SubscriptionStoreControlPlacement protocol.

## Topics

### Getting automatic placements

static var automatic: AutomaticSubscriptionStoreControlPlacement

A context-appropriate placement that the system determines automatically.

static var bottomBar: AutomaticSubscriptionStoreControlPlacement

A placement that locates the subscription controls in a bar near the bottom of the main scroll view in a subscription store view.

static var buttonsInBottomBar: AutomaticSubscriptionStoreControlPlacement

A hybrid placement that positions subscription controls within the main scroll view, and places auxiliary buttons in the bottom bar.

static var scrollView: AutomaticSubscriptionStoreControlPlacement

A placement that locates the subscription controls within the main scroll view of a subscription store view.

static var bottom: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the bottom edge of the view.

static var leading: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the leading edge of the view.

static var trailing: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the trailing edge of the view.

## Relationships

### Conforms To

- RawRepresentable
- SubscriptionStoreControlPlacement

## See Also

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

