

- HealthKit
- HKUnit
-  atmosphere() 

Type Method

# atmosphere()

Returns a HealthKit unit for measuring pressure in atmospheres.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func atmosphere() -> Self
```

## Return Value

A HealthKit unit for measuring pressure in atmospheres.

## Discussion

One atmosphere is the average atmospheric pressure at sea level.

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

class func centimeterOfWater() -> Self

Returns a HealthKit unit for measuring pressure in centimeters of water.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

