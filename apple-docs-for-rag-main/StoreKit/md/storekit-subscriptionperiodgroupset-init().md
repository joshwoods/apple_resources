

- StoreKit
- SubscriptionPeriodGroupSet
-  init() 

Initializer

# init()

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init() where Label == AutomaticSubscriptionOptionGroupLabel, MarketingContent == AutomaticSubscriptionStoreMarketingContent
```

## See Also

### Creating subscription period group sets

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent)

init(marketingContent: (Product.SubscriptionPeriod?) -> MarketingContent, label: (Product.SubscriptionPeriod?) -> Label)

