

- HealthKit
- HKUnit
-  stone() 

Type Method

# stone()

Returns a HealthKit unit for measuring mass in stones.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func stone() -> Self
```

## Return Value

A HealthKit unit for measuring mass in stones.

## See Also

### Constructing mass units

class func gram() -> Self

Returns a HealthKit unit for measuring mass in grams.

class func gramUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring mass, using gram units with the provided prefix.

class func ounce() -> Self

Returns a HealthKit unit for measuring mass in ounces.

class func pound() -> Self

Returns a HealthKit unit for measuring mass in pounds.

class func moleUnit(withMolarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

class func moleUnit(with: HKMetricPrefix, molarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

