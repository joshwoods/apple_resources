

- HealthKit
- HKCategoryTypeIdentifier
-  appleStandHour 

Type Property

# appleStandHour

A category sample type that counts the number of hours in the day during which the user has stood and moved for at least one minute per hour.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let appleStandHour: HKCategoryTypeIdentifier
```

## Discussion

This quantity type counts the number of hours during which the user stood and moved for at least one minute per hour.

If wheelchairUse() returns HKWheelchairUse.yes, Apple Watch calculates the number of hours during which the user rolled for at least one minute instead. Also, the Activity rings display Roll hours instead of Stand hours.

Note

Roll hours are recorded using the appleStandHours quantity type. Check the wheelchairUse() method’s return value to determine whether the data should be interpreted as Roll or Stand hours.

These samples use values from the HKCategoryValueAppleStandHour enumeration. They represent the data tracked by the Stand ring on Apple Watch.

## See Also

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

