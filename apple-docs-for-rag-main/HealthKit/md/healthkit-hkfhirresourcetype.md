

- HealthKit
-  HKFHIRResourceType 

Structure

# HKFHIRResourceType

The FHIR resource types supported in HealthKit.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
struct HKFHIRResourceType
```

## Mentioned in 

Accessing Health Records

## Topics

### Resource Types

static let allergyIntolerance: HKFHIRResourceType

A type that identifies FHIR resources for allergies and intolerances.

static let condition: HKFHIRResourceType

A type that identifies FHIR resources for a condition, problem, diagnosis, or other event.

static let diagnosticReport: HKFHIRResourceType

A type that identifies FHIR resources for findings and interpretation of diagnostic tests.

static let documentReference: HKFHIRResourceType

A type that identifies FHIR resources for document references.

static let immunization: HKFHIRResourceType

A type that identifies FHIR resources for the administration of vaccines.

static let medicationOrder: HKFHIRResourceType

A type that identifies FHIR resources for prescriptions or other orders for medication.

static let medicationDispense: HKFHIRResourceType

A type that identifies FHIR resources for the delivery of medication (usually in response to a prescription).

static let medicationStatement: HKFHIRResourceType

A type that identifies FHIR resources for statements about medication taken by the patient.

static let medicationRequest: HKFHIRResourceType

A type that identifies FHIR resources for prescriptions or other orders or requests for medication.

static let observation: HKFHIRResourceType

A type that identifies FHIR resources for medical observations, including lab results and vital signs.

static let procedure: HKFHIRResourceType

A type that identifies FHIR resources for procedures performed on the patient.

static let coverage: HKFHIRResourceType

A type that identifies FHIR resources containing information about the user’s insurance coverage.

### Initializers

init(rawValue: String)

Returns a new resource type for the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing FHIR Data

var identifier: String

The value from the FHIR resource’s `id` field.

var fhirVersion: HKFHIRVersion

The FHIR version used by this resource.

class HKFHIRVersion

The FHIR version.

var resourceType: HKFHIRResourceType

The value from the FHIR resource’s `resourceType` field.

var sourceURL: URL?

The full URL for the source of the FHIR resource.

var data: Data

The JSON representation of the FHIR resource.

