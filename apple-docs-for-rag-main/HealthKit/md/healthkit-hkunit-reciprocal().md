

- HealthKit
- HKUnit
-  reciprocal() 

Instance Method

# reciprocal()

Returns a complex unit representing the unit’s reciprocal.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
func reciprocal() -> HKUnit
```

## Return Value

A complex unit that is the reciprocal of the unit the method was called on.

## Discussion

This method creates a new, complex unit by dividing 1 by the unit the method was called on. This is often only one step in a series of operations. For example, you can use this method to create a meters-per-second unit, as shown below.

- Swift
- Objective-C

```
let meters = HKUnit.meterUnit()
let seconds = HKUnit.secondUnit()
let secondsInverse = seconds.reciprocalUnit()
let metersPerSecond = meters.unitMultipliedByUnit(secondsInverse)
```

```
HKUnit *meters = [HKUnit meterUnit];
HKUnit *seconds = [HKUnit secondUnit];
HKUnit *secondsInverse = [seconds reciprocalUnit];
HKUnit *metersPerSecond = [meters unitMultipliedByUnit:secondsInverse];
```

## See Also

### Related Documentation

convenience init(from: String)

Returns the unit instance described by the provided string.

### Performing unit math

func unitMultiplied(by: HKUnit) -> HKUnit

Creates a complex unit by multiplying the receiving unit with another unit.

func unitDivided(by: HKUnit) -> HKUnit

Creates a complex unit by dividing the receiving unit by another unit.

func unitRaised(toPower: Int) -> HKUnit

Creates a complex unit by raising the unit to the given power.

