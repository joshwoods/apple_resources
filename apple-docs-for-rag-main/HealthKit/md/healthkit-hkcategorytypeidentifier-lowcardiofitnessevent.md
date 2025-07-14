

- HealthKit
- HKCategoryTypeIdentifier
-  lowCardioFitnessEvent 

Type Property

# lowCardioFitnessEvent

An event that indicates the user’s VO2 max values consistently fall below a particular aerobic fitness threshold.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 13.0+visionOS 1.0+watchOS 7.2+

``` source
static let lowCardioFitnessEvent: HKCategoryTypeIdentifier
```

## Discussion

In iOS 14.3 and later, users with a paired Apple Watch running watchOS 7.2 or later can enable a Health app experience that classifies their cardio fitness levels as either “Low”, “Below Average”, “Above Average”, or “High”, based on individual parameters and characteristics.

Apple Watch can notify the user when their cardio fitness level falls into the Low category. If the user enables these notifications, they receive a notification when their VO2 max levels consistently fall below the low threshold for a period of time. The system sends low-cardio fitness notifications approximately once every four months.

The system also creates a lowCardioFitnessEvent sample to record the event. The sample contains values from the HKCategoryValueLowCardioFitnessEvent enumeration.

Samples of this type have two associated metadata keys:

HKMetadataKeyVO2MaxValue  
This key stores the value of the VO2 max sample that triggered the event.

HKMetadataKeyLowCardioFitnessEventThreshold  
This key stores the threshold value used to calculate the Low cardio classification. This value varies based on certain parameters and physical characteristics, such as the user’s age.

Low-cardio fitness event samples are read-only. Use this identifier to request permission to read these samples; however, you can’t request authorization to share them, and you can’t save new low-cardio fitness event samples to the HealthKit store.

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

