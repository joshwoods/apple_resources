

- HealthKit
-  HKPredicateKeyPathCategoryValue 

Global Variable

# HKPredicateKeyPathCategoryValue

The key path for accessing the category sample’s value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKPredicateKeyPathCategoryValue: String
```

## Discussion

Use this constant whenever you want to include a sample’s quantity in a predicate format string. Add a `%K` placeholder to the format string, and then pass this constant as an argument.

