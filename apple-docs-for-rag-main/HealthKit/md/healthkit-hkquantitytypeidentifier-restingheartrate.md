

- HealthKit
- HKQuantityTypeIdentifier
-  restingHeartRate 

Type Property

# restingHeartRate

A quantity sample type that measures the user’s resting heart rate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
static let restingHeartRate: HKQuantityTypeIdentifier
```

## Discussion

These samples use count/time units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle).

Resting heart rate is commonly correlated with overall cardiovascular health. It is an estimation of the user’s lowest heart rate during periods of rest, and is intended to be used as a medically relevant metric. A resting heart rate sample is different than a sedentary heart rate sample (that is, a sample using the heartRate identifier with a HKHeartRateMotionContext.sedentary motion context). For example, if the user finishes a high-intensity workout, and then sits down to rest, the next heart rate sample may be marked as a sedentary sample, but it is still much higher than the user’s actual resting heart rate. To produce more accurate results, the system estimates the resting heart rate by analyzing sedentary heart rate samples throughout the day.

Because the resting heart rate estimates become more accurate as the day progresses, the system may delete earlier samples and replace them with better estimates. Apple Watch replaces only the samples written by the watch for the current or previous day.

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

static let heartRateVariabilitySDNN: HKQuantityTypeIdentifier

A quantity sample type that measures the standard deviation of heartbeat intervals.

static let heartRateRecoveryOneMinute: HKQuantityTypeIdentifier

A quantity sample that records the reduction in heart rate from the peak exercise rate to the rate one minute after exercising ended.

static let atrialFibrillationBurden: HKQuantityTypeIdentifier

A quantity type that measures an estimate of the percentage of time a person’s heart shows signs of atrial fibrillation (AFib) while wearing Apple Watch.

static let walkingHeartRateAverage: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate while walking.

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

