

- StoreKit
- SubscriptionPeriodGroupSet
-  init(marketingContent:) 

Initializer

# init(marketingContent:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(@ViewBuilder marketingContent: @escaping (Product.SubscriptionPeriod?) -> MarketingContent) where Label == AutomaticSubscriptionOptionGroupLabel
```

## See Also

### Creating subscription period group sets

init()

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent, label: (Product.SubscriptionPeriod?) -> Label)

