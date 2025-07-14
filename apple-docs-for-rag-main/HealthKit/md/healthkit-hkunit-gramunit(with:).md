

- HealthKit
- HKUnit
-  gramUnit(with:) 

Type Method

# gramUnit(with:)

Returns a HealthKit unit for measuring mass, using gram units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func gramUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring mass based on grams and the given prefix.

## Discussion

This method is used to create prefixed versions of grams, typically kilogram units, as shown below.

- Swift
- Objective-C

```
let kg = HKUnit.gramUnitWithMetricPrefix(.Kilo)
let kg = HKUnit.gramUnitWithMetricPrefix(.Kilo)
```

```
HKUnit *kg = [HKUnit gramUnitWithMetricPrefix:HKMetricPrefixKilo];
```

## See Also

### Constructing mass units

class func gram() -> Self

Returns a HealthKit unit for measuring mass in grams.

class func ounce() -> Self

Returns a HealthKit unit for measuring mass in ounces.

class func pound() -> Self

Returns a HealthKit unit for measuring mass in pounds.

class func stone() -> Self

Returns a HealthKit unit for measuring mass in stones.

class func moleUnit(withMolarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

class func moleUnit(with: HKMetricPrefix, molarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

