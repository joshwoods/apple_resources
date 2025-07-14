

- StoreKit
- SubscriptionPeriodGroupSet
-  init(marketingContent:label:) 

Initializer

# init(marketingContent:label:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    @ViewBuilder marketingContent: @escaping (Product.SubscriptionPeriod?) -> MarketingContent,
    @ViewBuilder label: @escaping (Product.SubscriptionPeriod?) -> Label
)
```

## See Also

### Creating subscription period group sets

init()

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent)

