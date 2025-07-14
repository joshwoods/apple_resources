

- HealthKit
-  HKMetadataKeyBloodGlucoseMealTime 

Global Variable

# HKMetadataKeyBloodGlucoseMealTime

A key that indicates the relative timing of a blood glucose reading to a meal.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
let HKMetadataKeyBloodGlucoseMealTime: String
```

## Discussion

Set this key on a bloodGlucose sample. Set it’s value to an NSNumber object containing a HKBloodGlucoseMealTime value.Medical professionals can use the relative meal time to help determine the acceptable range for a blood glucose reading. If your app requires more precise timing or additional information about the meal’s composition, create samples to record those details (for example, a dietaryCarbohydrates sample with the exact meal time).

## Topics

### Valid Values

enum HKBloodGlucoseMealTime

Constants indicating the timing of a blood glucose sample relative to a meal.

