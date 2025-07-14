

- HealthKit
-  HKCategorySample 

Class

# HKCategorySample

A sample with values from a short list of possible values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCategorySample
```

## Mentioned in 

About the HealthKit framework

Saving data to HealthKit

## Overview

You can use category samples to record sleep data using the HKCategoryValueSleepAnalysis enumeration. Individual samples represent time periods when the user is in bed or asleep. Samples with different values may have overlapping time intervals. For example, when the user is both in bed and asleep, create an in-bed sample and an asleep sample with overlapping times.

The HKCategorySample class is a concrete subclass of the HKSample class. Category samples are immutable: You set the sample’s properties when you create it, and they can’t change.

### Extend Category Samples

Like many HealthKit classes, don’t subclass the `HKCategorySample` class. You may extend the `HKCategorySample` class by adding metadata with custom keys as appropriate for your app.

For more information, see init(type:value:start:end:metadata:).

## Topics

### Creating Category Samples

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date)

Creates a newly instantiated category sample.

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date, metadata: [String : Any]?)

Creates a newly instantiated category sample with the provided metadata.

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

Creates a newly instantiated category sample including the provided device and metadata.

### Getting Property Data

var categoryType: HKCategoryType

The category type for this sample.

var value: Int

The category value for this sample.

### Assigning Values

enum HKCategoryValue

Categories that are undefined.

enum HKCategoryValueCervicalMucusQuality

Categories that represent the user’s cervical mucus quality.

enum HKCategoryValueMenstrualFlow

Categories that indicate the amount of menstrual flow for a given sample.

Deprecated

enum HKCategoryValueOvulationTestResult

Categories that represent the result of an ovulation home test.

enum HKCategoryValueContraceptive

The type of contraceptive.

enum HKCategoryValueSleepAnalysis

Categories that represent the result of a sleep analysis.

enum HKCategoryValueAppetiteChanges

Categories that represent change in appetite.

enum HKCategoryValuePresence

Categories that indicate whether a symptom is present.

enum HKCategoryValueSeverity

Categories that represent the severity of a symptom.

enum HKCategoryValueEnvironmentalAudioExposureEvent

Exposure events for environmental audio.

enum HKCategoryValueHeadphoneAudioExposureEvent

Exposure events for headphone audio.

enum HKCategoryValueLowCardioFitnessEvent

A value that indicates a low-level cardio fitness event.

enum HKAppleWalkingSteadinessClassification

A classification of a score based on the steadiness of the user’s gait.

enum HKCategoryValueAppleWalkingSteadinessEvent

The value of an event triggered by a reduced score for the steadiness of the user’s gait.

enum HKCategoryValuePregnancyTestResult

Category values that indicate the results of a home pregnancy test.

enum HKCategoryValueProgesteroneTestResult

A category value that indicates the result from a home progesterone test.

enum HKCategoryValueAudioExposureEvent

Categories that indicate audio exposure events.

Deprecated

### Specifying Predicate Key Paths

let HKPredicateKeyPathCategoryValue: String

The key path for accessing the category sample’s value.

## Relationships

### Inherits From

- HKSample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Basic samples

class HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.

Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

