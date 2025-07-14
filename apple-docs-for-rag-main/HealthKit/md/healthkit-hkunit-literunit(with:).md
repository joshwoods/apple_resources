

- HealthKit
- HKUnit
-  literUnit(with:) 

Type Method

# literUnit(with:)

Returns a HealthKit unit for measuring volume, using liter units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func literUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring volume based on liters and the provided prefix.

## Discussion

This method is used to create prefixed versions of liters, typically milliliter units, as shown below.

- Swift
- Objective-C

```
let ml = HKUnit.literUnitWithMetricPrefix(.Milli)
let ml = HKUnit.literUnitWithMetricPrefix(.Milli)
```

```
HKUnit *ml = [HKUnit literUnitWithMetricPrefix:HKMetricPrefixMilli];
```

## See Also

### Constructing volume units

class func liter() -> Self

Returns a HealthKit unit for measuring volume in liters.

class func fluidOunceUS() -> Self

Returns a HealthKit unit for measuring volume in US fluid ounces.

class func fluidOunceImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial fluid ounces.

class func cupUS() -> Self

Returns a HealthKit unit for measuring volume in US cups.

class func cupImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial cups.

class func pintUS() -> Self

Returns a HealthKit unit for measuring volume in US pints.

class func pintImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial pints.

