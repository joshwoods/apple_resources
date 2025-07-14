

- StoreKit
- SubscriptionOptionGroup
-  init(isIncluded:label:) 

Initializer

# init(isIncluded:label:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    isIncluded: @escaping (Product) -> Bool,
    @ViewBuilder label: () -> Label
) where Content == Never
```

Available when `Content` conforms to `StoreContent`, `Label` conforms to `View`, and `MarketingContent` is `AutomaticSubscriptionStoreMarketingContent`.

## See Also

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

init(isIncluded: (Product) -> Bool, label: () -> Label, marketingContent: () -> MarketingContent)

init(isIncluded: (Product) -> Bool, marketingContent: () -> MarketingContent)

