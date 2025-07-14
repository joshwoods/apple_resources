

- HealthKit
- HKUnit
-  unitDivided(by:) 

Instance Method

# unitDivided(by:)

Creates a complex unit by dividing the receiving unit by another unit.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
func unitDivided(by unit: HKUnit) -> HKUnit
```

## Parameters 

`unit`  

The unit to be divided.

## Return Value

A new, complex unit.

## Discussion

This method creates a new, complex unit by dividing one unit by another. For example, you can create a meters-per-second unit by dividing a meters unit by a seconds unit, as shown below.

- Swift
- Objective-C

```
let meters = HKUnit.meterUnit()
let seconds = HKUnit.secondUnit()
let metersPerSecond = meters.unitDividedByUnit(seconds)
```

```
HKUnit *meters = [HKUnit meterUnit];
HKUnit *seconds = [HKUnit secondUnit];
HKUnit *metersPerSecond = [meters unitDividedByUnit:seconds];
```

## See Also

### Related Documentation

convenience init(from: String)

Returns the unit instance described by the provided string.

### Performing unit math

func unitMultiplied(by: HKUnit) -> HKUnit

Creates a complex unit by multiplying the receiving unit with another unit.

func unitRaised(toPower: Int) -> HKUnit

Creates a complex unit by raising the unit to the given power.

func reciprocal() -> HKUnit

Returns a complex unit representing the unit’s reciprocal.

