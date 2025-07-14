

- HealthKit
- Samples
-  Accessing Data from a SMART Health Card 

Sample Code

# Accessing Data from a SMART Health Card

Query for and validate a verifiable clinical record.

Download

iOS 15.0+iPadOS 15.0+Xcode 13.3+

## Overview

Note

This sample code project is associated with WWDC21 session 10089: Explore Verifiable Health Records.

### Configure the Sample Code Project

Before you run the sample code project in Xcode:

- In Simulator, open Safari, and navigate to `https://spec.smarthealth.cards/examples/`.

- Download one of the SMART Health Cards (like `example-00-e-file.smart-health-card`).

- After the file downloads, tap the download arrow, then select Downloads from the pop-up menu. You can also find the downloaded SMART Health Cards in Files (Browse \> On My iPhone \> Downloads).

- Select the health card, and follow the instructions to add the card to Health.

## See Also

### Medical records

Accessing Health Records

Read clinical record data from the HealthKit store.

Accessing Sample Data in the Simulator

Set up sample accounts to build and test your app.

Accessing a User’s Clinical Records

Request authorization to query HealthKit for a user’s clinical records and display them in your app.

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

class HKDocumentSample

An abstract class that represents a health document in the HealthKit store.

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

class HKDocumentType

A sample type used to create queries for documents.

