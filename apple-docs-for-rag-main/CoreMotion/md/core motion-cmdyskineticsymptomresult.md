

- Core Motion
-  CMDyskineticSymptomResult 

Class

# CMDyskineticSymptomResult

A result object that contains data about the likely presence of dyskinetic symptoms during a one-minute interval.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+watchOS 5.0+

``` source
class CMDyskineticSymptomResult
```

## Mentioned in 

Getting movement disorder symptom data

## Overview

Dyskinesias are uncontrolled, involuntary movements that occur as a side effect of taking Levadopa to control Parkinson’s disease. Dyskinesias can manifest in a single body part, such as the arm, leg, or head, or they can affect the entire body. Particular dyskinesias resemble actions like fidgeting, writhing, wriggling, head bobbing, or body swaying. These symptoms tend to occur during the drug’s peak dosage. Dyskinesias typically occur in patients with advanced Parkinson’s disease, who may require higher dosages of Levadopa.

The following equation is always true: percentUnlikely `+` percentLikely `= 1.0`.

Important

Gather and present data on dyskinetic symptom results only to users with choreiform dyskinesias, either self-reported or diagnosed by a clinician.

## Topics

### Reading the Time Interval

var startDate: Date

The result’s start time and date.

var endDate: Date

The result’s end time and date.

### Accessing Dyskinetic Symptom Data

var percentUnlikely: Float

The percentage of time when dyskinetic symptoms were unlikely.

var percentLikely: Float

The percentage of time when dyskinetic symptoms were likely.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Movement disorder

Getting movement disorder symptom data

Retrieve data from the Apple Watch’s movement disorder manager.

Adhering to the movement disorder data collection requirements

Ensure that your users understand and have control over the data your app collects.

Movement disorder algorithm changelog

A chronological log of notable changes to the movement disorder algorithm.

class CMMovementDisorderManager

A manager for recording and querying movement disorder data.

class CMTremorResult

A result object that contains data about the presence and strength of tremors during a one-minute interval.

