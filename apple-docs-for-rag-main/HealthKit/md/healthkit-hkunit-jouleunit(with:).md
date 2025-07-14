

- HealthKit
- HKUnit
-  jouleUnit(with:) 

Type Method

# jouleUnit(with:)

Returns a HealthKit unit for measuring energy, using joule units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func jouleUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring energy based on joules and the provided prefix.

## Discussion

This method is used to create prefixed versions of joules. HealthKit commonly uses kilojoules to measure food energy in many regions. Kilojoules can be created as shown below.

- Swift
- Objective-C

```
let kj = HKUnit.jouleUnitWithMetricPrefix(.Kilo)
```

```
HKUnit *kj = [HKUnit jouleUnitWithMetricPrefix:HKMetricPrefixKilo];
```

## See Also

### Constructing energy units

class func joule() -> Self

Returns a HealthKit unit for measuring energy in joules.

class func kilocalorie() -> Self

Returns a HealthKit unit for measuring energy in kilocalories.

class func largeCalorie() -> Self

Returns a HealthKit unit for measuring energy in large calories (Cal).

class func smallCalorie() -> Self

Returns a HealthKit unit for measuring energy in small calories (cal).

class func calorie() -> Self

Returns a HealthKit unit for measuring energy in calories.

Deprecated

