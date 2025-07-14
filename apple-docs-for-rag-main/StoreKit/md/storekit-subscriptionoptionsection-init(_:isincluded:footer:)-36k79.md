

- StoreKit
- SubscriptionOptionSection
-  init(\_:isIncluded:footer:) 

Initializer

# init(\_:isIncluded:footer:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ title: some StringProtocol,
    isIncluded: @escaping (Product) -> Bool,
    @ViewBuilder footer: () -> Footer = EmptyView.init
)
```

Available when `Header` is `Text`, `Content` is `Never`, and `Footer` conforms to `View`.

## See Also

### Creating subscription option sections

init(LocalizedStringKey, isIncluded: (Product) -> Bool, footer: () -> Footer)

init(isIncluded: (Product) -> Bool, header: () -> Header, footer: () -> Footer)

