

- HealthKit
-  HKCategoryValueAppleWalkingSteadinessEvent 

Enumeration

# HKCategoryValueAppleWalkingSteadinessEvent

The value of an event triggered by a reduced score for the steadiness of the user’s gait.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
enum HKCategoryValueAppleWalkingSteadinessEvent
```

## Overview

These values indicate that the user received a Low or Very Low score for their Walking Steadiness. The HKCategoryValueAppleWalkingSteadinessEvent.repeatLow and HKCategoryValueAppleWalkingSteadinessEvent.repeatVeryLow values indicate that the Low and Very Low scores persisted over a significant period of time.

## Topics

### Steadiness Values

case initialLow

The user received a below-normal steadiness score for their gait while walking.

case initialVeryLow

The user received a steadiness score for their gait while walking that was considerably below normal.

case repeatLow

The user’s below-normal score persists over a significant period of time.

case repeatVeryLow

The user’s considerably below-normal score persists over a significant period of time.

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

enum HKCategoryValuePregnancyTestResult

Category values that indicate the results of a home pregnancy test.

enum HKCategoryValueProgesteroneTestResult

A category value that indicates the result from a home progesterone test.

