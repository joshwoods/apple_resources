

- StoreKit
- SubscriptionOptionSection
-  init(isIncluded:header:footer:) 

Initializer

# init(isIncluded:header:footer:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    isIncluded: @escaping (Product) -> Bool,
    @ViewBuilder header: () -> Header = EmptyView.init,
    @ViewBuilder footer: () -> Footer = EmptyView.init
)
```

Available when `Header` conforms to `View`, `Content` is `Never`, and `Footer` conforms to `View`.

## See Also

### Creating subscription option sections

init(LocalizedStringKey, isIncluded: (Product) -> Bool, footer: () -> Footer)

init(some StringProtocol, isIncluded: (Product) -> Bool, footer: () -> Footer)

