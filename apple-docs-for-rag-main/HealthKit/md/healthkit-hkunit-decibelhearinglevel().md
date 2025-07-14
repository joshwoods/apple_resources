

- HealthKit
- HKUnit
-  decibelHearingLevel() 

Type Method

# decibelHearingLevel()

Returns a HealthKit unit for measuring the intensity of a sound.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func decibelHearingLevel() -> Self
```

## Discussion

This unit measures the intensity of the sound relative to the quietest sound a typical young, healthy individual can hear.

## See Also

### Related Documentation

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

