

- HealthKit
- HKQuantity
-  compare(\_:) 

Instance Method

# compare(\_:)

Compares two values after converting them to the same units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(_ quantity: HKQuantity) -> ComparisonResult
```

## Parameters 

`quantity`  

The quantity to compare. This method throws an exception if the quantities do not have compatible units (invalidArgumentException).

## Return Value

ComparisonResult.orderedDescending if the parameter is less than the receiver. ComparisonResult.orderedAscending if the parameter is greater than the receiver. ComparisonResult.orderedSame if the quantities are equal.

## Discussion

Returns whether the quantity argument is less than, equal to, or greater than the current quantity. This method automatically converts the quantities into the same units before comparing the values. You just need to ensure that the quantities have compatible units.

Note

Converting a value to a different unit can introduce floating point errors. Values that should be equal may appear unequal due to these floating point errors.

In most cases, the compatible units are clear from context. To see the unit types associated with different quantity sample types, see the type identifiers in HKQuantityTypeIdentifier.

If you need to programmatically check whether a particular unit is compatible with a particular quantity, call the quantity’s is(compatibleWith:) method.

## See Also

### Related Documentation

func `is`(compatibleWith: HKUnit) -> Bool

Returns a boolean value indicating whether the quantity is compatible with the provided unit.

