

- HealthKit
-  HKMetadataKeySwimmingLocationType 

Global Variable

# HKMetadataKeySwimmingLocationType

A key that indicates the location for a swimming workout.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
let HKMetadataKeySwimmingLocationType: String
```

## Discussion

Set this key on a workout object that represents swimming. Set its value to an NSNumber object that contains a valid value from the HKWorkoutSwimmingLocationType enumeration.

## Topics

### Valid Swimming Locations

enum HKWorkoutSwimmingLocationType

The possible locations for swimming.

## See Also

### Swimming

let HKMetadataKeySwimmingStrokeStyle: String

A key that indicates the predominant stroke style for a lap of swimming.

let HKMetadataKeyLapLength: String

A key that indicates the length of a lap during a workout.

let HKMetadataKeySWOLFScore: String

let HKMetadataKeyWaterSalinity: String

