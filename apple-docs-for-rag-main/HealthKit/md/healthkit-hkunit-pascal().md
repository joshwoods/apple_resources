

- HealthKit
- HKUnit
-  pascal() 

Type Method

# pascal()

Returns a HealthKit unit for measuring pressure in pascals.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func pascal() -> Self
```

## Return Value

A HealthKit unit for measuring pressure in pascals.

## See Also

### Constructing pressure units

class func pascalUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

class func millimeterOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in millimeters of mercury.

class func inchesOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in inches of mercury.

class func centimeterOfWater() -> Self

Returns a HealthKit unit for measuring pressure in centimeters of water.

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

