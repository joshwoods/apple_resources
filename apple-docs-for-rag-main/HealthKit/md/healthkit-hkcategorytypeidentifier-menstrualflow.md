

- HealthKit
- HKCategoryTypeIdentifier
-  menstrualFlow 

Type Property

# menstrualFlow

A category sample type that records menstrual cycles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let menstrualFlow: HKCategoryTypeIdentifier
```

## Discussion

These samples use values from the HKCategoryValueMenstrualFlow enum. Additionally, these samples must include HKMetadataKeyMenstrualCycleStart metadata.

When recording data about the user’s menstrual cycle, you can either use a single sample for the entire period, or multiple samples to record changes over the cycle. When using single samples, pass the start of the menstrual period to the `startDate` parameter. Pass the end of the period to the `endDate` parameter, and set the HKMetadataKeyMenstrualCycleStart value to true.

When using multiple samples to record a single period, the `startDate` and `endDate` parameters should mark the beginning and ending of each individual sample. Set the HKMetadataKeyMenstrualCycleStart value for the first sample in the period to true. Use false for any additional samples. Different samples can use different `menstrualFlow` values to record the changes in flow over time.

## Topics

### Metadata Keys

let HKMetadataKeyMenstrualCycleStart: String

A key that indicates whether the sample represents the start of a menstrual cycle. This metadata key is required for menstrualFlow category samples.

## See Also

### Related Documentation

enum HKCategoryValue

Categories that are undefined.

struct HKCategoryTypeIdentifier

Identifiers for creating category types.

class HKCategoryType

A type that identifies samples that contain a value from a small set of possible values.

class HKCategorySample

A sample with values from a short list of possible values.

### Reproductive health

static let intermenstrualBleeding: HKCategoryTypeIdentifier

A category sample type that records spotting outside the normal menstruation period.

static let infrequentMenstrualCycles: HKCategoryTypeIdentifier

A category sample that indicates an infrequent menstrual cycle.

static let irregularMenstrualCycles: HKCategoryTypeIdentifier

A category sample that indicates an irregular menstrual cycle.

static let persistentIntermenstrualBleeding: HKCategoryTypeIdentifier

A category sample that indicates persistent intermenstrual bleeding.

static let prolongedMenstrualPeriods: HKCategoryTypeIdentifier

A category sample that indicates a prolonged menstrual cycle.

static let basalBodyTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the user’s basal body temperature.

static let cervicalMucusQuality: HKCategoryTypeIdentifier

A category sample type that records the quality of the user’s cervical mucus.

static let ovulationTestResult: HKCategoryTypeIdentifier

A category sample type that records the result of an ovulation home test.

static let progesteroneTestResult: HKCategoryTypeIdentifier

A category type that represents the results from a home progesterone test.

static let sexualActivity: HKCategoryTypeIdentifier

A category sample type that records sexual activity.

static let contraceptive: HKCategoryTypeIdentifier

A category sample type that records the use of contraceptives.

static let pregnancy: HKCategoryTypeIdentifier

A category type that records pregnancy.

static let pregnancyTestResult: HKCategoryTypeIdentifier

A category type that represents the results from a home pregnancy test.

static let lactation: HKCategoryTypeIdentifier

A category type that records lactation.

