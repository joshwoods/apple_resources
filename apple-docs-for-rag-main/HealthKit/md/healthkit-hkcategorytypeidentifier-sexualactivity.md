

- HealthKit
- HKCategoryTypeIdentifier
-  sexualActivity 

Type Property

# sexualActivity

A category sample type that records sexual activity.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let sexualActivity: HKCategoryTypeIdentifier
```

## Discussion

Use a HKCategoryValue.notApplicable value with these samples. These samples can include HKMetadataKeySexualActivityProtectionUsed metadata.

## Topics

### Metadata Keys

let HKMetadataKeySexualActivityProtectionUsed: String

A key that indicates whether protection was used during sexual activity. This metadata key can be used with sexualActivity category samples.

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

static let menstrualFlow: HKCategoryTypeIdentifier

A category sample type that records menstrual cycles.

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

static let contraceptive: HKCategoryTypeIdentifier

A category sample type that records the use of contraceptives.

static let pregnancy: HKCategoryTypeIdentifier

A category type that records pregnancy.

static let pregnancyTestResult: HKCategoryTypeIdentifier

A category type that represents the results from a home pregnancy test.

static let lactation: HKCategoryTypeIdentifier

A category type that records lactation.

