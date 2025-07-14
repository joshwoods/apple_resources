

- HealthKit
- HKClinicalTypeIdentifier
-  clinicalNoteRecord 

Type Property

# clinicalNoteRecord

A type identifier for records of clinical notes.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+watchOS 9.4+

``` source
static let clinicalNoteRecord: HKClinicalTypeIdentifier
```

## Discussion

Clinical notes can have one or more attached files. While these files are often PDFs, HTML, or text files, they can be any format. Check the HKAttachment object’s contentType property to determine the file type. For more information on accessing the attachments, see HKAttachment.

If your app has permission to read clinicalNoteRecord samples, it can also access the attachments. For more information on reading clinical note records, see Accessing Health Records.

## See Also

### Related Documentation

class HKClinicalType

A type that identifies samples that contain clinical record data.

static let documentReference: HKFHIRResourceType

A type that identifies FHIR resources for document references.

static let diagnosticReport: HKFHIRResourceType

A type that identifies FHIR resources for findings and interpretation of diagnostic tests.

### Clinical Record Type Identifiers

static let allergyRecord: HKClinicalTypeIdentifier

A type identifier for records of allergic or intolerant reactions.

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

