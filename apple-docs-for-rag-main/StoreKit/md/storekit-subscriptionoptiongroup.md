

- StoreKit
-  SubscriptionOptionGroup 

Structure

# SubscriptionOptionGroup

A group of subscription options that includes optional views for labels and marketing content.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
struct SubscriptionOptionGroup where Content : StoreContent, Label : View, MarketingContent : View
```

## Topics

### Creating subscription option groups

init(LocalizedStringKey, content: () -> Content)

init(some StringProtocol, content: () -> Content)

init(LocalizedStringKey, content: () -> Content, marketingContent: () -> MarketingContent)

init(some StringProtocol, content: () -> Content, marketingContent: () -> MarketingContent)

init(LocalizedStringKey, isIncluded: (Product) -> Bool)

init(some StringProtocol, isIncluded: (Product) -> Bool)

init(LocalizedStringKey, isIncluded: (Product) -> Bool, marketingContent: () -> MarketingContent)

init(some StringProtocol, isIncluded: (Product) -> Bool, marketingContent: () -> MarketingContent)

init(content: () -> Content)

init(content: () -> Content, label: () -> Label)

init(content: () -> Content, label: () -> Label, marketingContent: () -> MarketingContent)

init(content: () -> Content, marketingContent: () -> MarketingContent)

init(isIncluded: (Product) -> Bool)

init(isIncluded: (Product) -> Bool, label: () -> Label)

init(isIncluded: (Product) -> Bool, label: () -> Label, marketingContent: () -> MarketingContent)

init(isIncluded: (Product) -> Bool, marketingContent: () -> MarketingContent)

### Supporting types

struct AutomaticSubscriptionOptionGroupLabel

## Relationships

### Conforms To

- Sendable
- StoreContent

## See Also

### Declaring the structure of a subscription store

struct SubscriptionOptionGroupSet

A set of groups of subscription options that include optional views for labels and marketing content.

struct SubscriptionPeriodGroupSet

struct SubscriptionOptionSection

protocol StoreContent

A type that represents the content of a store.

struct StoreContentBuilder

A result builder that creates store content from closures that you provide.

