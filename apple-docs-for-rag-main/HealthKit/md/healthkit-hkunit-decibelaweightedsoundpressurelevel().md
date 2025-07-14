

- HealthKit
- HKUnit
-  decibelAWeightedSoundPressureLevel() 

Type Method

# decibelAWeightedSoundPressureLevel()

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func decibelAWeightedSoundPressureLevel() -> Self
```

## See Also

### Related Documentation

class func decibelHearingLevel() -> Self

Returns a HealthKit unit for measuring the intensity of a sound.

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

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

