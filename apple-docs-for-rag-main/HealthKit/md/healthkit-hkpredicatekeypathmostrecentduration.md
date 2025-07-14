

- HealthKit
-  HKPredicateKeyPathMostRecentDuration 

Global Variable

# HKPredicateKeyPathMostRecentDuration

A key path for the duration of the sample’s most recent quantity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let HKPredicateKeyPathMostRecentDuration: String
```

## Discussion

Use this constant whenever you want to include a sample’s quantity in a predicate format string. Add a `%K` placeholder to the format string, and then pass this constant as an argument.

## See Also

### Specifying Predicate Key Paths

let HKPredicateKeyPathMin: String

The key path for the sample’s minimum quantity.

let HKPredicateKeyPathAverage: String

The key path for the sample’s average quantity.

let HKPredicateKeyPathMax: String

The key path for the sample’s maximum quantity.

let HKPredicateKeyPathMostRecent: String

The key path for the sample’s most recent quantity.

let HKPredicateKeyPathMostRecentStartDate: String

The key path for the start date of the sample’s most recent quantity.

let HKPredicateKeyPathMostRecentEndDate: String

The key path for the end date of the sample’s most recent quantity.

