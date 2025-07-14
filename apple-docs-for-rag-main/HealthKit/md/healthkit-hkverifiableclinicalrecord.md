

- HealthKit
-  HKVerifiableClinicalRecord 

Class

# HKVerifiableClinicalRecord

A sample that represents the contents of a SMART Health Card or EU Digital COVID Certificate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
class HKVerifiableClinicalRecord
```

## Overview

HKVerifiableClinicalRecord samples contain data from a SMART Health Card or EU Digital COVID Certificate. Verifiable clinical records combine information about the user’s identity with clinical data, like an immunization record or a lab test result. The organization that produced the data cryptographically signs the bundle.

Apps that use verifiable clinical records can use the cryptographic signature to verify the authenticity of the contents. To verify the card:

1.  Access the card’s raw payload using the clinical record’s dataRepresentation property.

2.  Unzip the payload and parse out the `iss` value, which contains a URL that identifies the organization that issued the card.

3.  Get the public key from the issuer.

4.  Verify the payload’s signature.

For more information, see SMART Health Cards Framework and Electronic Health Certificates. You can download example SMART cards for testing and development from Examples.

## Topics

### Identifying the Subject

var subject: HKVerifiableClinicalRecordSubject

Data about the person whose clinical data the card contains.

### Identifying the Issuer

var issuerIdentifier: String

An identifier that represents the card’s issuer.

### Reading Metadata

var issuedDate: Date

The date when the issuer created the card.

var relevantDate: Date

A date relevant to this record, such as when the issuer administered a vaccine or performed a test.

var expirationDate: Date?

The date when the card expires.

var recordTypes: [String]

An array of strings representing the types of records contained in the card.

var sourceType: HKVerifiableClinicalRecordSourceType?

The source for the verifiable clinical record

struct HKVerifiableClinicalRecordSourceType

The source type for the verifiable clinical record.

var itemNames: [String]

A human-readable description of the card’s contents.

### Accessing the Raw Payload

var dataRepresentation: Data

A raw representation of the record’s data.

var jwsRepresentation: Data

A raw representation of the SMART Health Card’s contents.

Deprecated

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

