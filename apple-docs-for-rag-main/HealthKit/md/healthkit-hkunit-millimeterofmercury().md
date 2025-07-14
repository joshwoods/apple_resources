

- HealthKit
- HKUnit
-  millimeterOfMercury() 

Type Method

# millimeterOfMercury()

Returns a HealthKit unit for measuring pressure in millimeters of mercury.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func millimeterOfMercury() -> Self
```

## Return Value

A HealthKit unit for measuring pressure in millimeters of mercury.

## Discussion

One millimeter of mercury is the pressure needed to raise a column of mercury by 1 millimeter. Even through it is not an SI unit, the millimeter of mercury unit is used in many scientific fields. In HealthKit, it is commonly used to measure blood pressure.

## See Also

### Constructing pressure units

class func pascal() -> Self

Returns a HealthKit unit for measuring pressure in pascals.

class func pascalUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

class func inchesOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in inches of mercury.

class func centimeterOfWater() -> Self

Returns a HealthKit unit for measuring pressure in centimeters of water.

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

