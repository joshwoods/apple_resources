

- StoreKit
-  SubscriptionPeriodGroupSet 

Structure

# SubscriptionPeriodGroupSet

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct SubscriptionPeriodGroupSet where Label : View, MarketingContent : View
```

## Topics

### Creating subscription period group sets

init()

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent)

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent, label: (Product.SubscriptionPeriod?) -> Label)

### Creating the group style

nonisolated func subscriptionStoreOptionGroupStyle(_ style: some SubscriptionOptionGroupStyle) -> some View 

Sets the style subscription store views within this view use to display groups of subscription options.

## Relationships

### Conforms To

- Sendable
- StoreContent

## See Also

### Declaring the structure of a subscription store

struct SubscriptionOptionGroup

A group of subscription options that includes optional views for labels and marketing content.

struct SubscriptionOptionGroupSet

A set of groups of subscription options that include optional views for labels and marketing content.

struct SubscriptionOptionSection

protocol StoreContent

A type that represents the content of a store.

struct StoreContentBuilder

A result builder that creates store content from closures that you provide.

