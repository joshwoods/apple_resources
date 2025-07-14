

- HealthKit
- HKQuantityTypeIdentifier
-  basalBodyTemperature 

Type Property

# basalBodyTemperature

A quantity sample type that records the user’s basal body temperature.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let basalBodyTemperature: HKQuantityTypeIdentifier
```

## Discussion

Basal body temperature measures the body’s temperature when at rest (for example, taking the temperature immediately after waking). These samples use temperature units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle).

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

