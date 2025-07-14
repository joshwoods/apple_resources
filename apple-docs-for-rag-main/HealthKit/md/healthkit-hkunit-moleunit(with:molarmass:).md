

- HealthKit
- HKUnit
-  moleUnit(with:molarMass:) 

Type Method

# moleUnit(with:molarMass:)

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func moleUnit(
    with prefix: HKMetricPrefix,
    molarMass gramsPerMole: Double
) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

`gramsPerMole`  

The molar mass, in grams per mole, of the item to be weighed.

## Return Value

A HealthKit unit for measuring mass in moles.

## Discussion

This method allows the creation of units to measure mass in moles with a given metric prefix and molecular mass. For example, to measure blood glucose in millimoles, you need to use both the correct prefix (milli-) and the HKUnitMolarMassBloodGlucose constant.).

- Swift
- Objective-C

```
let millimolesOfBloodGlucose =
    HKUnit.moleUnitWithMetricPrefix(HKMetricPrefix.Milli,
                                    molarMass: HKUnitMolarMassBloodGlucose)
```

```
HKUnit *millimolesOfBloodGlucose =
[HKUnit moleUnitWithMetricPrefix:HKMetricPrefixMilli molarMass:HKUnitMolarMassBloodGlucose];
```

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

class func stone() -> Self

Returns a HealthKit unit for measuring mass in stones.

class func moleUnit(withMolarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

