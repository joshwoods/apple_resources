

- HealthKit
-  Samples 

API Collection

# Samples

Create and save health and fitness samples.

## Overview

The HealthKit store saves most health and fitness data using HKSample subclasses. All sample subclasses record information at a specified time. If the sample’s startDate and endDate properties are the same, the sample represents a point in time. If the endDate is after the startDate, the sample represents a time interval.

HealthKit uses different HKSample subclasses to store different types of data:

- HKQuantitySample objects store quantities—a numerical value and units. Most HealthKit data types use quantity samples. For example, height, heart rate, and dietary energy consumed all use quantity samples.

- HKCategorySample objects store a single option selected from a short list. For example, category samples record sleep data (the user can be in bed, asleep, or awake).

- HKCorrelation samples combine two or more samples into a single value. For example, correlation samples represent food intake and blood pressure samples. A food sample contains any number of nutrition samples, while a blood pressure sample contains both a systolic and a diastolic sample.

- HealthKit represents specialized data types with sample subclasses such as HKCDADocumentSample, HKWorkoutRoute, and HKWorkout.

## Topics

### Essentials

Saving data to HealthKit

Create and share HealthKit samples.

Reading and Writing HealthKit Series Data

Share and read heartbeat and quantity series data using series builders and queries.

### Basic samples

class HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKCategorySample

A sample with values from a short list of possible values.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.

Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

### Series data

class HKQuantitySeriesSampleBuilder

A builder object for incrementally building a sample that contains multiple quantities.

class HKHeartbeatSeriesBuilder

A builder object for incrementally building a heartbeat series.

class HKHeartbeatSeriesSample

A sample that represents a series of heartbeats.

### Electrocardiograms

class HKElectrocardiogram

A sample for electrocardiogram data.

class VoltageMeasurement

The voltage for all leads at a single point in time.

### Audiograms

class HKAudiogramSample

A sample that stores an audiogram.

class HKAudiogramSensitivityPoint

A hearing sensitivity reading associated with a hearing test.

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

class HKDocumentSample

An abstract class that represents a health document in the HealthKit store.

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

class HKDocumentType

A sample type used to create queries for documents.

### Vision prescriptions

class HKVisionPrescription

A sample that stores a vision prescription.

class HKGlassesPrescription

A sample that stores a prescription for glasses.

class HKContactsPrescription

A sample that store a prescription for contacts.

class HKGlassesLensSpecification

An object that contains the glasses prescription data for one eye.

class HKContactsLensSpecification

An object that contains the contacts prescription data for one eye.

class HKLensSpecification

An abstract superclass for lens specifications.

class HKVisionPrism

Prescription data for eye alignment.

class HKPrescriptionType

A type that identifies samples that store a prescription.

### Walking steadiness classifications

enum HKAppleWalkingSteadinessClassification

A classification of a score based on the steadiness of the user’s gait.

HKAppleWalkingSteadinessClassificationForQuantity

Provides a classification for a score that measures the steadiness of the user’s gait.

HKAppleWalkingSteadinessMaximumQuantityForClassification

Returns the maximum score for the steadiness of the user’s gait based on the provided classification.

HKAppleWalkingSteadinessMinimumQuantityForClassification

Returns the minimum score for the steadiness of the user’s gait based on the provided classification.

### Attachments

class HKAttachment

A file that is attached to a sample in the HealthKit store.

class HKAttachmentStore

The access point for attachments associated with samples in the HealthKit store.

class HKAttachmentDataReader

A reader that provides access to an attachment’s data.

### Digital signatures

Adding Digital Signatures

Cryptographically sign samples.

### Abstract superclasses

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKSample

A HealthKit sample represents a piece of data associated with a start and end time.

class HKObject

A piece of data that can be stored inside the HealthKit store.

### Deprecated classes

class HKCumulativeQuantitySeriesSample

A sample representing a series of cumulative quantity values.

Deprecated

## See Also

### Health data

Saving data to HealthKit

Create and share HealthKit samples.

Reading data from HealthKit

Use queries to request sample data from HealthKit.

class HKHealthStore

The access point for all data managed by HealthKit.

Creating a Mobility Health App

Create a health app that allows a clinical care team to send and receive mobility data.

Data types

Specify the kind of data used in HealthKit.

Queries

Query health and fitness data.

Visualizing HealthKit State of Mind in visionOS

Incorporate HealthKit State of Mind into your app and visualize the data in visionOS.

