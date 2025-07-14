

- HealthKit
- HKUnit
-  inchesOfMercury() 

Type Method

# inchesOfMercury()

Returns a HealthKit unit for measuring pressure in inches of mercury.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class func inchesOfMercury() -> Self
```

## Return Value

A HealthKit unit for measuring pressure in inches of mercury.

## See Also

### Constructing pressure units

class func pascal() -> Self

Returns a HealthKit unit for measuring pressure in pascals.

class func pascalUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

class func millimeterOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in millimeters of mercury.

class func centimeterOfWater() -> Self

Returns a HealthKit unit for measuring pressure in centimeters of water.

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

