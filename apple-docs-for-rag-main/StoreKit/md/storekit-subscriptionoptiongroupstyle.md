

- StoreKit
-  SubscriptionOptionGroupStyle 

Protocol

# SubscriptionOptionGroupStyle

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol SubscriptionOptionGroupStyle
```

## Topics

### Getting built-in subscription option group styles

static var automatic: AutomaticSubscriptionOptionGroupStyle

static var links: LinksSubscriptionOptionGroupStyle

static var tabs: TabsSubscriptionOptionGroupStyle

### Supporting types

struct AutomaticSubscriptionOptionGroupStyle

struct LinksSubscriptionOptionGroupStyle

struct TabsSubscriptionOptionGroupStyle

struct SubscriptionOptionGroupStyleOutput

## Relationships

### Conforming Types

- AutomaticSubscriptionOptionGroupStyle
- LinksSubscriptionOptionGroupStyle
- TabsSubscriptionOptionGroupStyle

## See Also

### Styling subscription option groups

nonisolated func subscriptionStoreOptionGroupStyle(_ style: some SubscriptionOptionGroupStyle) -> some View 

Sets the style subscription store views within this view use to display groups of subscription options.

func subscriptionStoreOptionGroupStyle(some SubscriptionOptionGroupStyle) -> some StoreContent

