

- StoreKit
-  SubscriptionStoreButton 

Structure

# SubscriptionStoreButton

A button for subscribing to an in-app subscription with a localized label and optional caption.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct SubscriptionStoreButton
```

## Overview

When implementing custom subscription store control styles conforming to SubscriptionStoreControlStyle, you can use this button to utilize the standard subscribe button as a component of the view you provide from makeBody(configuration:). The subscription store button automatically generates a localized label and optional caption for the corresponding subscription option. To configure a custom button label, use Button instead.

Standard subscription store control styles use the subscription store button. For example, the buttons style creates a `SubscriptionStoreButton` instance for each subscription option.

Tip

Within the scope of your type conforming to SubscriptionStoreControlStyle, you can spell `SubscriptionStoreButton` as `SubscribeButton` through the SubscriptionStoreControlStyle.SubscribeButton type alias.

In iOS, macOS, visionOS and watchOS you can configure the button’s label by modifying it with `subscriptionStoreButtonLabel(_:)`. Some button label configurations cause the button to have a caption, for example .`displayName.singleLine`.

Because the `SubscriptionStoreButton` is composed of a SwiftUI Button, you can also configure the button using other built-in view modifiers such as buttonStyle(_:).

To create a `SubscriptionStoreButton`, provide a value of SubscriptionStoreControlStyleConfiguration.Option to the init(_:) method. Get an option value from the required makeBody(configuration:) method on your SubscriptionStoreControlStyle implementation.

Important

Use `SubscriptionStoreButton` only in the view you return from the required makeBody(configuration:) method of SubscriptionStoreControlStyle. Using `SubscriptionStoreButton` in other contexts is not supported.

## Topics

### Creating a subscription store button

init(SubscriptionStoreControlStyleConfiguration.Option)

Creates a button with an automatic label that describes the subscription option and starts a subscribe interaction when someone selects the button.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Creating custom subscription store control styles

struct SubscriptionStorePicker

A composite control with a picker for selecting a subscription option and a button for confirming the subscription.

struct SubscriptionStorePickerOption

A subscription option within a subscription picker control.

