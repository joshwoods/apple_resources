

- HealthKit
-  HKDocumentSample 

Class

# HKDocumentSample

An abstract class that represents a health document in the HealthKit store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
class HKDocumentSample
```

## Overview

You should never instantiate an `HKDocumentSample` object directly. Instead, you always work with a concrete subclass. In iOS 10 and watchOS 3, the only concrete class is the HKCDADocumentSample class.

Document samples are immutable: You set the sample’s properties when you create it, and they cannot change.

### Extend Document Samples

Like many HealthKit classes, you should not create any custom subclasses of the `HKDocumentSample` class. You can extend the `HKDocumentSample` class and its subclasses by adding custom metadata keys and values to the metadata dictionary when the object is instantiated.

## Topics

### Accessing the Document Sample Properties

var documentType: HKDocumentType

The type of document represented by the sample.

## Relationships

### Inherits From

- HKSample

### Inherited By

- HKCDADocumentSample

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

class HKVerifiableClinicalRecord

A sample that represents the contents of a SMART Health Card or EU Digital COVID Certificate.

class HKVerifiableClinicalRecordSubject

The subject associated with a signed clinical record.

class HKCDADocumentSample

A Clinical Document Architecture (CDA) sample that stores a single document.

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

class HKDocumentType

A sample type used to create queries for documents.

