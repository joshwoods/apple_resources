

- HealthKit
-  HKWorkoutSwimmingLocationType 

Enumeration

# HKWorkoutSwimmingLocationType

The possible locations for swimming.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
enum HKWorkoutSwimmingLocationType
```

## Topics

### Swimming Locations

case openWater

The user swam in open water like a lake or ocean.

case pool

The user swam in a pool.

case unknown

The swimming location could not be determined.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Session settings

var activityType: HKWorkoutActivityType

The workout session’s activity type.

var locationType: HKWorkoutSessionLocationType

The workout session’s location.

enum HKWorkoutSessionLocationType

A constant indicating whether the workout session takes place indoors or outdoors.

var swimmingLocationType: HKWorkoutSwimmingLocationType

The workout session’s swimming location.

var lapLength: HKQuantity?

The length of the lap for a workout session.

