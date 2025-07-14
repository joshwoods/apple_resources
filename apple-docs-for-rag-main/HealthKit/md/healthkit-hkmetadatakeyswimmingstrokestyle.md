

- HealthKit
-  HKMetadataKeySwimmingStrokeStyle 

Global Variable

# HKMetadataKeySwimmingStrokeStyle

A key that indicates the predominant stroke style for a lap of swimming.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
let HKMetadataKeySwimmingStrokeStyle: String
```

## Discussion

Set this key on workout lap events. Set its value to an NSNumber object that contains a valid value from the HKSwimmingStrokeStyle enumeration.

## Topics

### Valid Stroke Styles

enum HKSwimmingStrokeStyle

The style of stroke while swimming.

## See Also

### Swimming

let HKMetadataKeySwimmingLocationType: String

A key that indicates the location for a swimming workout.

let HKMetadataKeyLapLength: String

A key that indicates the length of a lap during a workout.

let HKMetadataKeySWOLFScore: String

let HKMetadataKeyWaterSalinity: String

