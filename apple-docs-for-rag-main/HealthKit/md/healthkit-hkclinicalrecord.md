

- HealthKit
-  HKClinicalRecord 

Class

# HKClinicalRecord

A sample that stores a clinical record.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
class HKClinicalRecord
```

## Mentioned in 

Accessing Health Records

Accessing Sample Data in the Simulator

## Overview

The clinical record stores information about a single condition, procedure, or result. While the record’s properties expose some high-level information, the fhirResource property contains the underlying data from the user’s healthcare institution.

Note that the record inherits the HKSample class’s startDate and endDate properties. However, the system does not populate these properties with information from the FHIR data; instead, the startDate and endDate reflect the time and date when the system downloaded the FHIR data to the device.

## Topics

### Accessing Clinical Record Data

var clinicalType: HKClinicalType

An identifier that indicates the type of record, such as an allergic reaction, a lab result, or a medical procedure.

var displayName: String

The primary display name as shown in the Health app.

var fhirResource: HKFHIRResource?

The Fast Healthcare Interoperability Resources (FHIR) data for this record.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Related Documentation

class HKClinicalType

A type that identifies samples that contain clinical record data.

### Medical records

Accessing Health Records

Read clinical record data from the HealthKit store.

Accessing Sample Data in the Simulator

Set up sample accounts to build and test your app.

Accessing a User’s Clinical Records

Request authorization to query HealthKit for a user’s clinical records and display them in your app.

Accessing Data from a SMART Health Card

Query for and validate a verifiable clinical record.

class HKFHIRResource

An object containing Fast Healthcare Interoperability Resources (FHIR) data.

class HKVerifiableClinicalRecord

A sample that represents the contents of a SMART Health Card or EU Digital COVID Certificate.

class HKVerifiableClinicalRecordSubject

The subject associated with a signed clinical record.

class HKCDADocumentSample

A Clinical Document Architecture (CDA) sample that stores a single document.

class HKDocumentSample

An abstract class that represents a health document in the HealthKit store.

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

class HKDocumentType

A sample type used to create queries for documents.

