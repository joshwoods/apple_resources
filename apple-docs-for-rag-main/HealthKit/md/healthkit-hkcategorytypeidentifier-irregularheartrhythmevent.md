

- HealthKit
- HKCategoryTypeIdentifier
-  irregularHeartRhythmEvent 

Type Property

# irregularHeartRhythmEvent

A category sample type for irregular heart rhythm events.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.2+

``` source
static let irregularHeartRhythmEvent: HKCategoryTypeIdentifier
```

## Discussion

The system creates irregularHeartRhythmEvent samples whenever Apple Watch produces an irregular rhythm notification. For more information, see Heart rate notifications on your Apple Watch.

The irregular rhythm samples are read-only. You can request permission to read the samples using this identifier, but you can’t request authorization to share them. This means you can’t save new irregular rhythm events to the HealthKit store. To add test data in iOS Simulator, open the Health app and select Browse \> Heart \> Irregular Rhythm Notifications \> Add Data.

These samples have a value of HKCategoryValue.notApplicable.

## See Also

### Vital signs

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

static let lowHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for low heart rate events.

static let highHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for high heart rate events.

static let restingHeartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s resting heart rate.

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

