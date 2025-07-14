

- HealthKit
-  HKFHIRResource 

Class

# HKFHIRResource

An object containing Fast Healthcare Interoperability Resources (FHIR) data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
class HKFHIRResource
```

## Mentioned in 

Accessing Health Records

## Topics

### Accessing FHIR Data

var identifier: String

The value from the FHIR resource’s `id` field.

var fhirVersion: HKFHIRVersion

The FHIR version used by this resource.

class HKFHIRVersion

The FHIR version.

var resourceType: HKFHIRResourceType

The value from the FHIR resource’s `resourceType` field.

struct HKFHIRResourceType

The FHIR resource types supported in HealthKit.

var sourceURL: URL?

The full URL for the source of the FHIR resource.

var data: Data

The JSON representation of the FHIR resource.

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

