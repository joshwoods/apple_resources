

- HealthKit
- HKUnit
-  unitRaised(toPower:) 

Instance Method

# unitRaised(toPower:)

Creates a complex unit by raising the unit to the given power.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
func unitRaised(toPower power: Int) -> HKUnit
```

## Parameters 

`power`  

The power by which to raise the unit.

## Return Value

A new, complex unit.

## Discussion

This method creates a new, complex unit by raising the unit this method is called on by the given power. This task is often only one step in a series of operations. For example, you can use this method to create a meters-per-second-squared unit as shown below.

- Swift
- Objective-C

```
let meters = HKUnit.meterUnit()
let seconds = HKUnit.secondUnit()
let squaredSeconds = seconds.unitRaisedToPower(2)
let metersPerSecondSquared = meters.unitDividedByUnit(squaredSeconds)
```

```
HKUnit *meters = [HKUnit meterUnit];
HKUnit *seconds = [HKUnit secondUnit];
HKUnit *squaredSeconds = [seconds unitRaisedToPower:2];
HKUnit *metersPerSecondSquared = [meters unitDividedByUnit:squaredSeconds];
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

func reciprocal() -> HKUnit

Returns a complex unit representing the unit’s reciprocal.

