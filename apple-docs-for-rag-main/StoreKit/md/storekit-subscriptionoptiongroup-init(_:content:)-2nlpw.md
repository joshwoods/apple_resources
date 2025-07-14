

- StoreKit
- SubscriptionOptionGroup
-  init(\_:content:) 

Initializer

# init(\_:content:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ label: LocalizedStringKey,
    @StoreContentBuilder content: () -> Content
)
```

Available when `Content` conforms to `StoreContent`, `Label` is `Text`, and `MarketingContent` is `AutomaticSubscriptionStoreMarketingContent`.

## See Also

### Creating subscription option groups

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

