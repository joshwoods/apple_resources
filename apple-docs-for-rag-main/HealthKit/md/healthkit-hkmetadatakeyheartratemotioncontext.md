

- HealthKit
-  HKMetadataKeyHeartRateMotionContext 

Global Variable

# HKMetadataKeyHeartRateMotionContext

The user’s activity level when the heart rate sample was measured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
let HKMetadataKeyHeartRateMotionContext: String
```

## Discussion

This key takes an NSNumber containing an HKHeartRateMotionContext as its value.

## Topics

### Valid Motion Contexts

enum HKHeartRateMotionContext

Values that indicate the user’s level of activity when the heart rate sample was measured.

## See Also

### Related Documentation

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

### Metadata Keys

let HKMetadataKeyHeartRateSensorLocation: String

The location where a specific heart rate reading was taken.

