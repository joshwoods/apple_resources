

- HealthKit
- HKCategoryTypeIdentifier
-  lowHeartRateEvent 

Type Property

# lowHeartRateEvent

A category sample type for low heart rate events.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.2+

``` source
static let lowHeartRateEvent: HKCategoryTypeIdentifier
```

## Discussion

The system creates lowHeartRateEvent samples whenever Apple Watch produces a low heart rate notification. For more information, see Heart rate notifications on your Apple Watch.

The low heart rate samples are read-only. You can request permission to read the samples using this identifier, but you can’t request authorization to share them. This means you can’t save new low heart rate events to the HealthKit store. To add test data in iOS Simulator, open the Health app and select Browse \> Heart \> Low Heart Rate Notifications \> Add Data.

These samples have a value of HKCategoryValue.notApplicable and include HKMetadataKeyHeartRateEventThreshold metadata.

## Topics

### Metadata Keys

let HKMetadataKeyHeartRateEventThreshold: String

A key that records the threshold of high or low heart rate events in beats per minute.

## See Also

### Vital signs

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

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

