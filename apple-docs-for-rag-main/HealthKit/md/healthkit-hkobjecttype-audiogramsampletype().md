

- HealthKit
- HKObjectType
-  audiogramSampleType() 

Type Method

# audiogramSampleType()

Returns an audiogram sample type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func audiogramSampleType() -> HKAudiogramSampleType
```

## Return Value

The shared HKAudiogramSampleType instance.

## Discussion

This method returns an instance of the HKAudiogramSampleType concrete subclass. HealthKit uses this type to store and read audiogram data from the HealthKit store.

