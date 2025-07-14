

- HealthKit
- HKHeartRateMotionContext
-  HKHeartRateMotionContext.notSet 

Case

# HKHeartRateMotionContext.notSet

A value indicating that the user’s activity level could not be determined.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
case notSet
```

## Discussion

This value is identical to the sample’s metadata not containing a HKMetadataKeyHeartRateMotionContext key.

## See Also

### Motion Contextes

case active

A value indicating that the user was in motion during the heart rate sample.

case sedentary

A value indicating that the user has been still for at least 5 minutes prior to the heart rate sample.

