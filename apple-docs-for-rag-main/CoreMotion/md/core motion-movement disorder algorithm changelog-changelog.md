

- Core Motion
-  Movement disorder algorithm changelog 

Article

# Movement disorder algorithm changelog

A chronological log of notable changes to the movement disorder algorithm.

## Overview

The movement disorder algorithm measures and records tremors and dyskinetic symptoms for Parkinson’s disease. For more information on receiving and using this data, see Getting movement disorder symptom data.

### Unreleased

- The version() method for checking the algorithm’s current version is available in watchOS 9.

### 1.0.0 — 2018-07-17

#### Added

- Released the algorithm used in watchOS 5 and later.

## See Also

### Movement disorder

Getting movement disorder symptom data

Retrieve data from the Apple Watch’s movement disorder manager.

Adhering to the movement disorder data collection requirements

Ensure that your users understand and have control over the data your app collects.

class CMMovementDisorderManager

A manager for recording and querying movement disorder data.

class CMTremorResult

A result object that contains data about the presence and strength of tremors during a one-minute interval.

class CMDyskineticSymptomResult

A result object that contains data about the likely presence of dyskinetic symptoms during a one-minute interval.

