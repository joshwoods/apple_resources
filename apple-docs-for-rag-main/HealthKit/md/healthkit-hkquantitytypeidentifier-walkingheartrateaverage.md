

- HealthKit
- HKQuantityTypeIdentifier
-  walkingHeartRateAverage 

Type Property

# walkingHeartRateAverage

A quantity sample type that measures the user’s heart rate while walking.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
static let walkingHeartRateAverage: HKQuantityTypeIdentifier
```

## Discussion

These samples use count/time units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle).

A user’s average heart rate while walking is correlated to their fitness level, because it corresponds to their heart’s efficiency while physically active. Apple Watch estimates the walking heart rate by averaging heart rate samples taken while the user is walking, as well as heart rate samples taken during walking workout sessions.

Because walking heart rate estimates become more accurate as the day progresses, the system may delete earlier samples and replace them with better estimates. Apple Watch replaces only the samples written by the watch for the current or previous day.

Note

Walking heart rate samples are automatically created by HealthKit. You cannot save your own walking heart rate samples; however, you can query these samples.

## See Also

### Vital signs

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

static let lowHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for low heart rate events.

static let highHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for high heart rate events.

static let irregularHeartRhythmEvent: HKCategoryTypeIdentifier

A category sample type for irregular heart rhythm events.

static let restingHeartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s resting heart rate.

static let heartRateVariabilitySDNN: HKQuantityTypeIdentifier

A quantity sample type that measures the standard deviation of heartbeat intervals.

static let heartRateRecoveryOneMinute: HKQuantityTypeIdentifier

A quantity sample that records the reduction in heart rate from the peak exercise rate to the rate one minute after exercising ended.

static let atrialFibrillationBurden: HKQuantityTypeIdentifier

A quantity type that measures an estimate of the percentage of time a person’s heart shows signs of atrial fibrillation (AFib) while wearing Apple Watch.

let HKDataTypeIdentifierHeartbeatSeries: String

A series sample containing heartbeat data.

class HKElectrocardiogramType

A type that identifies samples containing electrocardiogram data.

static let oxygenSaturation: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s oxygen saturation.

static let bodyTemperature: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s body temperature.

static let bloodPressure: HKCorrelationTypeIdentifier

A correlation sample that combines a systolic sample and a diastolic sample into a single blood pressure reading.

static let bloodPressureSystolic: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s systolic blood pressure.

static let bloodPressureDiastolic: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s diastolic blood pressure.

