

- HealthKit
- HKCategoryValuePredicateProviding
-  predicateForSamples(\_:value:) 

Type Method

# predicateForSamples(\_:value:)

Returns a predicate that checks a category sample’s value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
static func predicateForSamples(
    _ operatorType: NSComparisonPredicate.Operator,
    value: Self
) -> NSPredicate
```

Available when `RawValue` is `Int`.

## Parameters 

`operatorType`  

The type of operation to perform when matching the category sample’s value against the target value. For a list of possible operators, see NSComparisonPredicate.Operator.contains.

`value`  

The category sample’s target value. Use an enumeration value appropriate for the type of category samples you’re working with. For example, a predicate for sleep analysis samples use values from the HKCategoryValueSleepAnalysis enumeration.

## See Also

### Creating predicates

static func predicateForSamples(equalTo: Set&lt;Self>) -> NSPredicate

Returns a predicate that checks whether a category sample is equal to the provided set of values.

