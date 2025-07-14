

- HealthKit
- HKCategoryValuePredicateProviding
-  predicateForSamples(equalTo:) 

Type Method

# predicateForSamples(equalTo:)

Returns a predicate that checks whether a category sample is equal to the provided set of values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
static func predicateForSamples(equalTo values: Set) -> NSPredicate
```

Available when `RawValue` is `Int`.

## Parameters 

`values`  

The target set of values.

## See Also

### Creating predicates

static func predicateForSamples(NSComparisonPredicate.Operator, value: Self) -> NSPredicate

Returns a predicate that checks a category sample’s value.

