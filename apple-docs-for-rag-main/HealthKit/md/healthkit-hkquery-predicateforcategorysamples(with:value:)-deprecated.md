

- HealthKit
- HKQuery
-  predicateForCategorySamples(with:value:) Deprecated

Type Method

# predicateForCategorySamples(with:value:)

Returns a predicate that checks a category sample’s value.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+macOSvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func predicateForCategorySamples(
    with operatorType: NSComparisonPredicate.Operator,
    value: Int
) -> NSPredicate
```

Deprecated

Use predicateForSamples(_:value:) instead.

## Parameters 

`operatorType`  

The type of operation to perform when matching the category sample’s value against the target value. For a list of possible operators, see NSComparisonPredicate.Operator.contains.

`value`  

The category sample’s target value. Use an enumeration value appropriate for the type of category samples you are working with. For example, a predicate for sleep analysis samples use values from the HKCategoryValueSleepAnalysis enumeration.

## Return Value

A predicate that matches category samples based on the provided expression. This predicate works only with category samples.

## Discussion

Use this convenience method to create a predicate that checks a category sample’s value. The following listing uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let asleep = HKQuery.predicateForCategorySamplesWithOperatorType(
    .EqualToPredicateOperatorType,
    value: HKCategoryValueSleepAnalysis.Asleep.rawValue)

let explicitAsleep =
    NSPredicate(format: "%K == %d",
                HKPredicateKeyPathCategoryValue,
                HKCategoryValueSleepAnalysis.Asleep.rawValue)
```

```
NSPredicate *asleep =
    [HKQuery
     predicateForCategorySamplesWithOperatorType:NSEqualToPredicateOperatorType
     value:HKCategoryValueSleepAnalysisAsleep];

NSPredicate *explicitAsleep =
    [NSPredicate predicateWithFormat:@"%K == %d",
     HKPredicateKeyPathCategoryValue,
     HKCategoryValueSleepAnalysisAsleep];
```

## See Also

### Related Documentation

var value: Int

The category value for this sample.

let HKPredicateKeyPathCategoryValue: String

The key path for accessing the category sample’s value.

### Creating category sample predicates

protocol HKCategoryValuePredicateProviding

A protocol for objects that produce predicates that match category value samples.

