

- HealthKit
- HKUnit
-  meterUnit(with:) 

Type Method

# meterUnit(with:)

Returns a HealthKit unit for measuring length, using meter units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func meterUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring length based on meters and the provided prefix.

## Discussion

This method is used to create prefixed versions of meters. Common uses include creating kilometer and centimeter units, as shown below.

- Swift
- Objective-C

```
let km = HKUnit.meterUnitWithMetricPrefix(.Kilo)
let cm = HKUnit.meterUnitWithMetricPrefix(.Centi)
```

```
HKUnit *km = [HKUnit meterUnitWithMetricPrefix:HKMetricPrefixKilo];
HKUnit *cm = [HKUnit meterUnitWithMetricPrefix:HKMetricPrefixCenti];
```

## See Also

### Constructing length units

class func meter() -> Self

Returns a HealthKit unit for measuring length in meters.

class func inch() -> Self

Returns a HealthKit unit for measuring length in inches.

class func foot() -> Self

Returns a HealthKit unit for measuring length in feet.

class func yard() -> Self

Returns a HealthKit unit for measuring length in yards.

class func mile() -> Self

Returns a HealthKit unit for measuring length in miles.

