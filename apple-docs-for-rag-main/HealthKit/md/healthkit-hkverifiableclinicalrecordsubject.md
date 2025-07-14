

- HealthKit
-  HKVerifiableClinicalRecordSubject 

Class

# HKVerifiableClinicalRecordSubject

The subject associated with a signed clinical record.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
class HKVerifiableClinicalRecordSubject
```

## Overview

HKVerifiableClinicalRecordSubject objects contain data about the subject from a SMART Health Card. These cards combine both the user’s identity and clinical data into a cryptographically-signed bundle. To protect the subject’s privacy, SMART Health Cards provide the minimum required data. For more information, see SMART Health Cards Framework.

## Topics

### Accessing Patient Data

var fullName: String

The subject’s full name.

var dateOfBirthComponents: DateComponents?

The subject’s birthdate.

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
- Sendable

## See Also

### Medical records

Accessing Health Records

Read clinical record data from the HealthKit store.

Accessing Sample Data in the Simulator

Set up sample accounts to build and test your app.

Accessing a User’s Clinical Records

Request authorization to query HealthKit for a user’s clinical records and display them in your app.

Accessing Data from a SMART Health Card

Query for and validate a verifiable clinical record.

class HKClinicalRecord

A sample that stores a clinical record.

class HKFHIRResource

An object containing Fast Healthcare Interoperability Resources (FHIR) data.

class HKVerifiableClinicalRecord

A sample that represents the contents of a SMART Health Card or EU Digital COVID Certificate.

class HKCDADocumentSample

A Clinical Document Architecture (CDA) sample that stores a single document.

class HKDocumentSample

An abstract class that represents a health document in the HealthKit store.

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

class HKDocumentType

A sample type used to create queries for documents.

