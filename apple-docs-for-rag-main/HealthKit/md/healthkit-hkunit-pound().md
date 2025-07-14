

- HealthKit
- HKUnit
-  pound() 

Type Method

# pound()

Returns a HealthKit unit for measuring mass in pounds.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func pound() -> Self
```

## Return Value

A HealthKit unit for measuring mass in pounds.

## See Also

### Constructing mass units

class func gram() -> Self

Returns a HealthKit unit for measuring mass in grams.

class func gramUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring mass, using gram units with the provided prefix.

class func ounce() -> Self

Returns a HealthKit unit for measuring mass in ounces.

class func stone() -> Self

Returns a HealthKit unit for measuring mass in stones.

class func moleUnit(withMolarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

class func moleUnit(with: HKMetricPrefix, molarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

