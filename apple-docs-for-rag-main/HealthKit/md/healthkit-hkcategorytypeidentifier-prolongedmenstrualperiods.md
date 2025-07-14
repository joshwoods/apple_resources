

- HealthKit
- HKCategoryTypeIdentifier
-  prolongedMenstrualPeriods 

Type Property

# prolongedMenstrualPeriods

A category sample that indicates a prolonged menstrual cycle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
static let prolongedMenstrualPeriods: HKCategoryTypeIdentifier
```

## Discussion

HealthKit generates Cycle Deviation notifications based on the cycle data a person enters. HealthKit processes this data on their iOS device. If it detects a potential deviation, it sends a notification asking them to verify their logged cycle history. If the person confirms that their cycle history is accurate, HealthKit saves a corresponding sample of the detected Cycle Deviation to the HealthKit store.

Cycle Deviation notifications include:

Persistent spotting  
Persistent spotting, also known as irregular intermenstrual bleeding, is defined as spotting that occurs in at least two of your cycles in the last six months. HealthKit records verified instances using persistentIntermenstrualBleeding samples.

Prolonged periods  
Prolonged periods are defined as menstrual bleeding that lasts for ten or more days, and this has happened at least two times in the last six months. HealthKit records verified instances using prolongedMenstrualPeriods samples.

Irregular cycles  
An irregular cycle is defined as at least a seventeen-day difference between a person’s shortest and longest cycles over the last six months. HealthKit records verified instances using irregularMenstrualCycles samples.

Infrequent periods  
An infrequent period is defined as having a period one or two times in the last six months. HealthKit records verified instances using infrequentMenstrualCycles samples.

Use a HKCategoryValue.notApplicable value with these samples.

Important

These samples are read-only. You can request permission to read the samples using this identifier, but you can’t request authorization to share them. This means you can’t save new infrequent menstrual cycle samples to the HealthKit store.

## See Also

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

