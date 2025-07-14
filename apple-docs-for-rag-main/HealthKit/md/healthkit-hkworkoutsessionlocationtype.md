

- HealthKit
-  HKWorkoutSessionLocationType 

Enumeration

# HKWorkoutSessionLocationType

A constant indicating whether the workout session takes place indoors or outdoors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKWorkoutSessionLocationType
```

## Topics

### Constants

case unknown

It is not known whether the workout session is taking place indoors or outdoors.

case indoor

The workout session is indoors.

case outdoor

The workout session is outdoors.

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

var swimmingLocationType: HKWorkoutSwimmingLocationType

The workout session’s swimming location.

enum HKWorkoutSwimmingLocationType

The possible locations for swimming.

var lapLength: HKQuantity?

The length of the lap for a workout session.

