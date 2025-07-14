

- HealthKit
-  HKMetadataKeyHeartRateEventThreshold 

Global Variable

# HKMetadataKeyHeartRateEventThreshold

A key that records the threshold of high or low heart rate events in beats per minute.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.2+

``` source
let HKMetadataKeyHeartRateEventThreshold: String
```

## Discussion

The value for this key contains an HKQuantity object with count/time units, described in HKUnit. This metadata key is used by highHeartRateEvent and lowHeartRateEvent category samples.

