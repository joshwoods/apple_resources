

- HealthKit
- HKFHIRResourceType
-  medicationRequest 

Type Property

# medicationRequest

A type that identifies FHIR resources for prescriptions or other orders or requests for medication.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+

``` source
static let medicationRequest: HKFHIRResourceType
```

## Mentioned in 

Accessing Health Records

## Discussion

FHIR renamed the resource type for medication requests and orders. FHIR DSTU2 uses the medicationOrder resource type, while FHIR R4 uses the medicationRequest resource type.

## See Also

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

static let observation: HKFHIRResourceType

A type that identifies FHIR resources for medical observations, including lab results and vital signs.

static let procedure: HKFHIRResourceType

A type that identifies FHIR resources for procedures performed on the patient.

static let coverage: HKFHIRResourceType

A type that identifies FHIR resources containing information about the user’s insurance coverage.

