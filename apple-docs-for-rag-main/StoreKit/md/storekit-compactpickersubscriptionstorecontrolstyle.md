

- StoreKit
-  CompactPickerSubscriptionStoreControlStyle 

Structure

# CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact picker control, with a single button to subscribe.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
struct CompactPickerSubscriptionStoreControlStyle
```

## Overview

This style lays out the picker options in a horizontal stack, and it can scroll horizontally if the contents are wider than the container. This style is recommended when you expect your store to display two or three subscription options.

## Topics

### Getting the compact picker control style

static var compactPicker: CompactPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a compact control, with a single button to subscribe.

### Creating the style

init()

Creates a compact picker subscription store control style.

### Placing the controls

struct Placement

The placement of the compact subscription picker in a subscription store view.

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

struct PagedPickerSubscriptionStoreControlStyle

A subscription store control style that displays subscription plans as a paged picker control, with a single button to subscribe.

