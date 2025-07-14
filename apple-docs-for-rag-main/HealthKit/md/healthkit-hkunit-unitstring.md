

- HealthKit
- HKUnit
-  unitString 

Instance Property

# unitString

A string representation of the unit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var unitString: String { get }
```

## Discussion

This property contains a string using the format required by init(from:).

## See Also

### Related Documentation

func reciprocal() -> HKUnit

Returns a complex unit representing the unit’s reciprocal.

func unitMultiplied(by: HKUnit) -> HKUnit

Creates a complex unit by multiplying the receiving unit with another unit.

func unitRaised(toPower: Int) -> HKUnit

Creates a complex unit by raising the unit to the given power.

func unitDivided(by: HKUnit) -> HKUnit

Creates a complex unit by dividing the receiving unit by another unit.

### Working with units

convenience init(from: String)

Returns the unit instance described by the provided string.

func isNull() -> Bool

Returns a Boolean value indicating whether the unit is null.

