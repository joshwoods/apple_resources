

- HealthKit
- HKQuantityTypeIdentifier
-  heartRateRecoveryOneMinute 

Type Property

# heartRateRecoveryOneMinute

A quantity sample that records the reduction in heart rate from the peak exercise rate to the rate one minute after exercising ended.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
static let heartRateRecoveryOneMinute: HKQuantityTypeIdentifier
```

## Discussion

Heart rate recovery samples use count units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle). These samples always record a positive value.

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

