

- HealthKit
- HKQuantityTypeIdentifier
-  appleMoveTime 

Type Property

# appleMoveTime

A quantity sample type that measures the amount of time the user has spent performing activities that involve full-body movements during the specified day.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 13.0+visionOS 1.0+watchOS 7.4+

``` source
static let appleMoveTime: HKQuantityTypeIdentifier
```

## Discussion

appleMoveTime measures every full minute where the watch detects the user actively moving. Apple Watch uses the accelerometer and gyroscopes to detect activities that involve full-body movements, like walking, running, or playing in the playground.

For younger users, HealthKit’s activity summary can track move time instead of active energy burned:

- HealthKit automatically tracks move time for any users under 13 years old.

- Users 13 to 18 years old can choose whether to track move time or active calorie burn.

- All users over 18 years old track active calorie burn.

These samples use time units (described in HKUnit) and measure cumulative values (described in HKQuantityAggregationStyle).

## See Also

### Related Documentation

var activityMoveMode: HKActivityMoveMode

The move mode that they system used for this activity summary.

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKQuantity

An object that stores a value for a given unit.

### Activity

static let stepCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of steps the user has taken.

static let distanceWalkingRunning: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved by walking or running.

static let runningSpeed: HKQuantityTypeIdentifier

A quantity sample type that measures the runner’s speed.

static let runningStrideLength: HKQuantityTypeIdentifier

A quantity sample type that measures the distance covered by a single step while running.

static let runningPower: HKQuantityTypeIdentifier

A quantity sample type that measures the rate of work required for the runner to maintain their speed.

static let runningGroundContactTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the runner’s foot is in contact with the ground while running.

static let runningVerticalOscillation: HKQuantityTypeIdentifier

A quantity sample type measuring pelvis vertical range of motion during a single running stride.

static let distanceCycling: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved by cycling.

static let pushCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of pushes that the user has performed while using a wheelchair.

static let distanceWheelchair: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved using a wheelchair.

static let swimmingStrokeCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of strokes performed while swimming.

static let distanceSwimming: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved while swimming.

static let distanceDownhillSnowSports: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has traveled while skiing or snowboarding.

static let basalEnergyBurned: HKQuantityTypeIdentifier

A quantity sample type that measures the resting energy burned by the user.

static let activeEnergyBurned: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of active energy the user has burned.

