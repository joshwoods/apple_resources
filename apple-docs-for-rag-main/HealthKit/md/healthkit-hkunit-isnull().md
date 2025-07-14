

- HealthKit
- HKUnit
-  isNull() 

Instance Method

# isNull()

Returns a Boolean value indicating whether the unit is null.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func isNull() -> Bool
```

## Return Value

true if the unit is null; otherwise, false.

## Discussion

Null units occur only when you create compound units in which all the units cancel out. For example, if you tried to create a unit by dividing deciliters by liters (`dL/L`), you would end up with a null unit.

## See Also

### Working with units

convenience init(from: String)

Returns the unit instance described by the provided string.

var unitString: String

A string representation of the unit object.

