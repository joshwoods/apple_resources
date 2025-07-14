

- HealthKit
-  HKCategoryValueCervicalMucusQuality 

Enumeration

# HKCategoryValueCervicalMucusQuality

Categories that represent the user’s cervical mucus quality.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKCategoryValueCervicalMucusQuality
```

## Overview

These values are ordered from least-fertile (Dry) to most-fertile (EggWhite).

## Topics

### Constants

case dry

Little or no mucus.

case sticky

Sticky mucus.

case creamy

Creamy mucus.

case watery

Watery mucus.

case eggWhite

Mucus the color and consistency of egg whites.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- HKCategoryValuePredicateProviding
- Hashable
- RawRepresentable
- Sendable

## See Also

### Assigning Values

enum HKCategoryValue

Categories that are undefined.

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

