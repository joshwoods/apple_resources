

- HealthKit
- HKUnit
-  pascalUnit(with:) 

Type Method

# pascalUnit(with:)

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func pascalUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring pressure based on pascals and the provided prefix.

## See Also

### Constructing pressure units

class func pascal() -> Self

Returns a HealthKit unit for measuring pressure in pascals.

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

