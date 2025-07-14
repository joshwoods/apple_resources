

- HealthKit
-  HKCategoryValueSleepAnalysis 

Enumeration

# HKCategoryValueSleepAnalysis

Categories that represent the result of a sleep analysis.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKCategoryValueSleepAnalysis
```

## Mentioned in 

Saving data to HealthKit

## Overview

These values provide the set of valid categories for sleep tracking in HealthKit. To record a sleep sample, create an HKCategorySample using a sleepAnalysis identifier and a HKCategoryValueSleepAnalysis value.

```
let sleepSampleType = HKCategoryType(.sleepAnalysis)
let sleepCategory = HKCategoryValueSleepAnalysis.asleepDeep.rawValue
let deepSleepSample  = HKCategorySample(type: sleepSampleType,
                                        value:sleepCategory,
                                        start: startDate,
                                        end: endDate)
```

Each sleep analysis sample can have only one value. To track both the amount of time a person spends in bed and the quality and quantity of their sleep, use samples with overlapping times.

One set of samples tracks the amount of time the user spent in bed. Then, you can partition the in-bed time into a more-detailed set of samples. These detailed samples show when the user was awake, in core sleep, in deep sleep, or in rapid eye movement (REM) sleep. The detailed samples overlap the in-bed sample, but they don’t overlap each other.

Note

Samples recorded by Apple Watch only include awake samples that occur between two sleep samples. When reading sleep samples from HealthKit, there might not be any detailed samples that correspond to the beginning or ending of an in-bed sample.

By comparing the start and end times of these samples, apps can calculate secondary statistics. For example: the amount of time it took for the user to fall asleep, the percentage of sleep time spent in deep sleep, the number of times the user woke while in bed, and the total amount of time spent both in bed and asleep.

## Topics

### Values for Tracking Time In-Bed

case inBed

The user is in bed.

### Values for Tracking Sleep States

case awake

The user is awake.

case asleepCore

The user is in light or intermediate sleep.

case asleepDeep

The user is in deep sleep.

case asleepREM

The user is in REM sleep.

case asleepUnspecified

The user is asleep, but the specific stage isn’t known.

### Deprecated values

static var asleep: HKCategoryValueSleepAnalysis

The user is sleeping.

Deprecated

### Initializers

init?(rawValue: Int)

### Type Properties

static var allAsleepValues: Set&lt;HKCategoryValueSleepAnalysis>

A set of values that represents the possible stages of sleep.

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

enum HKCategoryValueCervicalMucusQuality

Categories that represent the user’s cervical mucus quality.

enum HKCategoryValueMenstrualFlow

Categories that indicate the amount of menstrual flow for a given sample.

Deprecated

enum HKCategoryValueOvulationTestResult

Categories that represent the result of an ovulation home test.

enum HKCategoryValueContraceptive

The type of contraceptive.

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

