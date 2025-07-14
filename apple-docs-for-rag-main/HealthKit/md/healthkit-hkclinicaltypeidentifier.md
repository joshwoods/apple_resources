

- HealthKit
-  HKClinicalTypeIdentifier 

Structure

# HKClinicalTypeIdentifier

A type identifier for the different categories of clinical records.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
struct HKClinicalTypeIdentifier
```

## Mentioned in 

Accessing Health Records

Authorizing access to health data

## Overview

Clinical record samples are read-only, so you can’t request authorization to share clinical record types. You can’t create or save new HKClinicalRecord objects.

For additional information, see Accessing Health Records.

## Topics

### Clinical Record Type Identifiers

static let allergyRecord: HKClinicalTypeIdentifier

A type identifier for records of allergic or intolerant reactions.

static let clinicalNoteRecord: HKClinicalTypeIdentifier

A type identifier for records of clinical notes.

static let conditionRecord: HKClinicalTypeIdentifier

A type identifier for records of a condition, problem, diagnosis, or other event.

static let immunizationRecord: HKClinicalTypeIdentifier

A type identifier for records of the current or historical administration of vaccines.

static let labResultRecord: HKClinicalTypeIdentifier

A type identifier for records of lab results.

static let medicationRecord: HKClinicalTypeIdentifier

A type identifier for records of medication.

static let procedureRecord: HKClinicalTypeIdentifier

A type identifier for records of procedures.

static let vitalSignRecord: HKClinicalTypeIdentifier

A type identifier for records of vital signs.

static let coverageRecord: HKClinicalTypeIdentifier

A type identifier for records containing information about the user’s insurance coverage.

### Initializers

init(rawValue: String)

Returns a new clinical record type identifier for the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

