

- HealthKit
- HKQuantityTypeIdentifier
-  vo2Max 

Type Property

# vo2Max

A quantity sample that measures the maximal oxygen consumption during exercise.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
static let vo2Max: HKQuantityTypeIdentifier
```

## Discussion

VO2max—the maximum amount of oxygen your body can consume during exercise— is a strong predictor of overall health. Clinical tests measure VO2max by having the patient exercise on a treadmill or bike, with an intensity that increases every few minutes until exhaustion.

On Apple Watch Series 3 or later, the system automatically saves vo2Max samples to HealthKit. The watch estimates the user’s VO2max based on data gathered while the user is walking or running outdoors. For more information, see Understand Estimated Test Results.

You can also create and save your own vo2Max samples—for example, when creating an app that records the results of tests performed in a clinic. When creating vo2Max samples, use the HKMetadataKeyVO2MaxTestType metadata key to specify the type of test used to generate the sample.

vo2Max samples use volume/mass/time units (described in HKUnit), measured in ml/kg /min. They measure discrete values (described in HKQuantityAggregationStyle).

### Understand Estimated Test Results

Apple Watch Series 3 and later estimates the user’s VO2max by measuring the user’s heart rate response to exercise. The system can generate VO2max samples after an outdoor walk, outdoor run, or hiking workout. During the outdoor activity, the user must cover relatively flat ground (a grade of less than 5% incline or decline) with adequate GPS, heart rate signal quality, and sufficient exertion. The user must maintain a heart rate approximately greater than or equal to 130% of their resting heart rate. The system can estimate VO2max ranges from 14-60 ml/kg/min

The user must wear their Apple Watch for at least one day before the system can generate the first vo2Max sample. Additionally, the system doesn’t generate a vo2Max sample on the user’s first workout. However, it can make estimates based on data collected outside a workout session.

Apple Watch estimates *VO2max* based on sub-maximal predictions rather than *peakVO2*. Users don’t need to achieve peak heart rate to receive an estimate; however, the system does need to estimate their peak heart rate. Users who take medications that may reduce their peak heart rate can toggle a medication switch in the Health app to enable more accurate VO2max estimates.

## Topics

### Metadata Keys

let HKMetadataKeyVO2MaxTestType: String

The method used to calculate the user’s VO2 max rate.

## See Also

### Related Documentation

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

