

- HealthKit
- HKQuantity
-  is(compatibleWith:) 

Instance Method

# is(compatibleWith:)

Returns a boolean value indicating whether the quantity is compatible with the provided unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func `is`(compatibleWith unit: HKUnit) -> Bool
```

## Parameters 

`unit`  

The target unit.

## Return Value

`Yes` if the quantity is compatible; otherwise, false.

## Discussion

Individual units are compatible if they measure the same feature. For example, all length units are compatible. All mass units are also compatible. However, a length unit is not compatible with a mass unit.

Complex units are compatible if the equation defining the units are compatible. Specifically, it must use the same operators, and the operands must be compatible. For example, meters per second and miles per hour are compatible. The left operands are both length units, the right operands are both time units and they all use a division operator.

## See Also

### Working With Units

func doubleValue(for: HKUnit) -> Double

Returns the quantity’s value in the provided unit.

