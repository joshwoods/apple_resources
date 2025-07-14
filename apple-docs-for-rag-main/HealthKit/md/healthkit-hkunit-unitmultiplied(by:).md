

- HealthKit
- HKUnit
-  unitMultiplied(by:) 

Instance Method

# unitMultiplied(by:)

Creates a complex unit by multiplying the receiving unit with another unit.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
func unitMultiplied(by unit: HKUnit) -> HKUnit
```

## Parameters 

`unit`  

The unit to be multiplied.

## Return Value

A new, complex unit.

## Discussion

You can create a complex unit by multiplying two units together. For example, you could create a foot-pound unit by multiplying a foot unit by a pound unit as shown below.

- Swift
- Objective-C

```
let foot = HKUnit.footUnit()
let pound = HKUnit.poundUnit()
let footPound = foot.unitMultipliedByUnit(pound)
```

```
HKUnit *foot = [HKUnit footUnit];
HKUnit *pound = [HKUnit poundUnit];
HKUnit *footPound = [foot unitMultipliedByUnit:pound];
```

## See Also

### Related Documentation

convenience init(from: String)

Returns the unit instance described by the provided string.

### Performing unit math

func unitDivided(by: HKUnit) -> HKUnit

Creates a complex unit by dividing the receiving unit by another unit.

func unitRaised(toPower: Int) -> HKUnit

Creates a complex unit by raising the unit to the given power.

func reciprocal() -> HKUnit

Returns a complex unit representing the unit’s reciprocal.

