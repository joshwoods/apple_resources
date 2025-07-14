

- HealthKit
- HKUnit
-  centimeterOfWater() 

Type Method

# centimeterOfWater()

Returns a HealthKit unit for measuring pressure in centimeters of water.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func centimeterOfWater() -> Self
```

## Return Value

A HealthKit unit for measuring pressure in centimeters of water.

## Discussion

One centimeter of water is the pressure needed to raise a column of water by 1 centimeter.

## See Also

### Constructing pressure units

class func pascal() -> Self

Returns a HealthKit unit for measuring pressure in pascals.

class func pascalUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

class func millimeterOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in millimeters of mercury.

class func inchesOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in inches of mercury.

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

