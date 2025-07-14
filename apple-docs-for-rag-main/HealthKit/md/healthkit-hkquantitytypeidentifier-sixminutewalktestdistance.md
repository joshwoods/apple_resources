

- HealthKit
- HKQuantityTypeIdentifier
-  sixMinuteWalkTestDistance 

Type Property

# sixMinuteWalkTestDistance

A quantity sample type that stores the distance a user can walk during a six-minute walk test.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
static let sixMinuteWalkTestDistance: HKQuantityTypeIdentifier
```

## Discussion

The standard six-minute walk test measures the maximum number of meters a user can walk on an unobstructed, flat course.

On Apple Watch Series 3 or later, the system automatically records a weekly sixMinuteWalkTestDistance sample. You can also create and save your own sixMinuteWalkTestDistance samples—for example, when creating an app that records the results of tests performed in a clinic.

sixMinuteWalkTestDistance samples use length units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle). For example, the following code creates a unit in meters.

```
let meters = HKUnit.meter()
```

### Understand Estimated Test Results

Each week, the system calculates the approximate result a user might receive from a six-minute walk test administered at a clinic. The system estimates the result using passively observed motion and workout data. The maximum estimated distance is 500m.

To record an estimate, the user must wear the watch at least 8 hours a day, 3 days a week. Additionally, the user must meet the 8-hour threshold at least 10 times over the previous 4 weeks.

Apple Watch produces the best results when the user’s expected six-minute walk distance is less than 500m, and the user wears a calibrated Apple Watch while performing a representative range of physical activities each day. For more information about calibrating Apple Watch, see Calibrating your Apple Watch for improved Workout and Activity accuracy.

If the watch isn’t calibrated, users can improve the accuracy of their results by carrying their iPhone on their hip or in their front pants pocket. The system uses the walkingSpeed samples automatically recorded by the phone to help calibrate the six-minute walk algorithm. The system may also use GPS from both iPhone and Apple Watch to improve the calibration.

Samples indicate whether the device was sufficiently calibrated to support an accurate estimate using the HKMetadataKeyAppleDeviceCalibrated metadata key.

## Topics

### Enabling Recalibration

com.apple.developer.healthkit.recalibrate-estimates

A Boolean value that determines whether your app can recalibrate the prediction algorithm used to calculate supported sample types.

### Accessing Estimate Dates

let HKMetadataKeyDateOfEarliestDataUsedForEstimate: String

The earliest date of data used to calculate the sample’s estimated value.

## See Also

### Mobility

static let appleWalkingSteadiness: HKQuantityTypeIdentifier

A quantity sample type that measures the steadiness of the user’s gait.

static let appleWalkingSteadinessEvent: HKCategoryTypeIdentifier

A category sample type that records an incident where the user showed a reduced score for their gait’s steadiness.

static let walkingSpeed: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s average speed when walking steadily over flat ground.

static let walkingStepLength: HKQuantityTypeIdentifier

A quantity sample type that measures the average length of the user’s step when walking steadily over flat ground.

static let walkingAsymmetryPercentage: HKQuantityTypeIdentifier

A quantity sample type that measures the percentage of steps in which one foot moves at a different speed than the other when walking on flat ground.

static let walkingDoubleSupportPercentage: HKQuantityTypeIdentifier

A quantity sample type that measures the percentage of time when both of the user’s feet touch the ground while walking steadily over flat ground.

static let stairAscentSpeed: HKQuantityTypeIdentifier

A quantity sample type measuring the user’s speed while climbing a flight of stairs.

static let stairDescentSpeed: HKQuantityTypeIdentifier

A quantity sample type measuring the user’s speed while descending a flight of stairs.

