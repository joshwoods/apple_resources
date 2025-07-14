

- StoreKit
-  SubscriptionOptionSection 

Structure

# SubscriptionOptionSection

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct SubscriptionOptionSection where Header : View, Content : StoreContent, Footer : View
```

## Topics

### Creating subscription option sections

init(LocalizedStringKey, isIncluded: (Product) -> Bool, footer: () -> Footer)

init(some StringProtocol, isIncluded: (Product) -> Bool, footer: () -> Footer)

init(isIncluded: (Product) -> Bool, header: () -> Header, footer: () -> Footer)

### Choosing a subscription option group style

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

struct SubscriptionPeriodGroupSet

protocol StoreContent

A type that represents the content of a store.

struct StoreContentBuilder

A result builder that creates store content from closures that you provide.

