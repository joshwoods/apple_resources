

- StoreKit
-  SubscriptionStorePolicyKind 

Structure

# SubscriptionStorePolicyKind

The type of policy, such as the terms of service or privacy policies.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SubscriptionStorePolicyKind
```

## Overview

To set the destination of a policy button in a SubscriptionStoreView, use subscriptionStorePolicyDestination(url:for:) or subscriptionStorePolicyDestination(for:destination:).

## Topics

### Getting policy types

static var privacyPolicy: SubscriptionStorePolicyKind

The privacy policy type.

static var termsOfService: SubscriptionStorePolicyKind

The terms of service policy type.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Configuring the subscription store policies

nonisolated func subscriptionStorePolicyDestination(for button: SubscriptionStorePolicyKind, @ViewBuilder destination: () -> some View) -> some View 

Configures a view as the destination for a policy button action in subscription store views.

nonisolated func subscriptionStorePolicyDestination(url: URL, for button: SubscriptionStorePolicyKind) -> some View 

Configures a URL as the destination for a policy button action in subscription store views.

nonisolated func subscriptionStorePolicyForegroundStyle(_ style: some ShapeStyle) -> some View 

Sets the style for the terms of service and privacy policy buttons within a subscription store view.

nonisolated func subscriptionStorePolicyForegroundStyle(_ primary: some ShapeStyle, _ secondary: some ShapeStyle) -> some View 

Sets the primary and secondary style for the terms of service and privacy policy buttons within a subscription store view.

