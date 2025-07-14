

- HealthKit
- HKQuantitySeriesSampleQuery
-  init(sample:quantityHandler:) Deprecated

Initializer

# init(sample:quantityHandler:)

Creates a new series query.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
init(
    sample quantitySample: HKQuantitySample,
    quantityHandler: @escaping (HKQuantitySeriesSampleQuery, HKQuantity?, Date?, Bool, (any Error)?) -> Void
)
```

Deprecated

Use init(quantityType:predicate:quantityHandler:) instead.

