

- HealthKit
-  HKCategoryTypeIdentifier 

Structure

# HKCategoryTypeIdentifier

Identifiers for creating category types.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKCategoryTypeIdentifier
```

## Overview

To create an HKCategoryType instance, pass an HKCategoryTypeIdentifier value to the categoryType(forIdentifier:) method.

For the complete list of quantity type identifiers, see Activity.

## Topics

### Activity

static let appleStandHour: HKCategoryTypeIdentifier

A category sample type that counts the number of hours in the day during which the user has stood and moved for at least one minute per hour.

static let lowCardioFitnessEvent: HKCategoryTypeIdentifier

An event that indicates the user’s VO2 max values consistently fall below a particular aerobic fitness threshold.

### Reproductive Health

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

### Hearing

static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from the environment.

enum HKCategoryValueEnvironmentalAudioExposureEvent

Exposure events for environmental audio.

static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from headphones.

enum HKCategoryValueHeadphoneAudioExposureEvent

Exposure events for headphone audio.

static let audioExposureEvent: HKCategoryTypeIdentifier

A category sample type for audio exposure events.

Deprecated

### Vital Signs

static let lowHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for low heart rate events.

static let highHeartRateEvent: HKCategoryTypeIdentifier

A category sample type for high heart rate events.

static let irregularHeartRhythmEvent: HKCategoryTypeIdentifier

A category sample type for irregular heart rhythm events.

### Mobility

static let appleWalkingSteadinessEvent: HKCategoryTypeIdentifier

A category sample type that records an incident where the user showed a reduced score for their gait’s steadiness.

### Symptoms

Symptom Type Identifiers

Identifiers for medical symptoms.

### Mindfulness and Sleep

static let mindfulSession: HKCategoryTypeIdentifier

A category sample type for recording a mindful session.

static let sleepAnalysis: HKCategoryTypeIdentifier

A category sample type for sleep analysis information.

### Self Care

static let toothbrushingEvent: HKCategoryTypeIdentifier

A category sample type for toothbrushing events.

static let handwashingEvent: HKCategoryTypeIdentifier

A category sample type for handwashing events.

### Initializers

init(rawValue: String)

Returns a newly initialized category type identifier using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating category types

class func categoryType(forIdentifier: HKCategoryTypeIdentifier) -> HKCategoryType?

Returns the shared category type for the provided identifier.

