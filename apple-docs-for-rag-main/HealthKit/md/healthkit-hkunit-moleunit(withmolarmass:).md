

- HealthKit
- HKUnit
-  moleUnit(withMolarMass:) 

Type Method

# moleUnit(withMolarMass:)

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func moleUnit(withMolarMass gramsPerMole: Double) -> Self
```

## Parameters 

`gramsPerMole`  

The molar mass (in g/mol) of the item to be weighed.

## Return Value

A HealthKit unit for measuring the mass of an item in moles.

## Discussion

To create a unit for measuring an item in moles, you need to know that item’s molar mass. For example, you can use the HKUnitMolarMassBloodGlucose constant to create the mole unit for blood glucose, as shown below.

- Swift
- Objective-C

```
let molesOfBloodGlucose = HKUnit.moleUnitWithMolarMass(HKUnitMolarMassBloodGlucose)
```

```
HKUnit *molesOfBloodGlucose =
[HKUnit moleUnitWithMolarMass:HKUnitMolarMassBloodGlucose];
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

class func moleUnit(with: HKMetricPrefix, molarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

