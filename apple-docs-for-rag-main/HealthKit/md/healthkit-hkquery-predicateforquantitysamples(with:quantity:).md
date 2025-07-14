

- HealthKit
- HKQuery
-  predicateForQuantitySamples(with:quantity:) 

Type Method

# predicateForQuantitySamples(with:quantity:)

Returns a predicate that matches samples based on the target quantity.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForQuantitySamples(
    with operatorType: NSComparisonPredicate.Operator,
    quantity: HKQuantity
) -> NSPredicate
```

## Parameters 

`operatorType`  

The operator type to use when comparing the sample’s quantity to the target quantity.

`quantity`  

The target quantity object.

## Return Value

A predicate that matches samples based on the target quantity. This predicate works only on quantity samples.

## Discussion

Use this convenience method to create a predicate that matches against a sample’s quantity. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let targetWeight = HKQuantity(unit: HKUnit.poundUnit(),
                              doubleValue: 150.0)

let underTargetWeight =
    HKQuery.predicateForQuantitySamplesWithOperatorType(
        .LessThanOrEqualToPredicateOperatorType,
        quantity: targetWeight)

let explicitUnderTargetWeight = NSPredicate(format: "%K 

```
HKQuantity *targetWeight =
[HKQuantity quantityWithUnit:[HKUnit poundUnit]
                 doubleValue:150.0];

NSPredicate *underTargetWeight =
[HKQuery predicateForQuantitySamplesWithOperatorType:
    NSLessThanOrEqualToPredicateOperatorType
    quantity:targetWeight];

NSPredicate *explicitUnderTargetWeight =
[NSPredicate predicateWithFormat:@"%K 

## See Also

### Related Documentation

let HKPredicateKeyPathQuantity: String

The key path for accessing the sample’s quantity.

var quantity: HKQuantity

The quantity for this sample.

