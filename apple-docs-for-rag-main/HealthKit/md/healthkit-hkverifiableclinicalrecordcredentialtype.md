

- HealthKit
-  HKVerifiableClinicalRecordCredentialType 

Structure

# HKVerifiableClinicalRecordCredentialType

The type of record returned by a verifiable clinical record query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+watchOS 8.5+

``` source
struct HKVerifiableClinicalRecordCredentialType
```

## Topics

### Identifying Record Types

static let covid19: HKVerifiableClinicalRecordCredentialType

A value that represents records about COVID-19.

static let immunization: HKVerifiableClinicalRecordCredentialType

A value that represents immunizations.

static let laboratory: HKVerifiableClinicalRecordCredentialType

A value that represents laboratory results.

static let recovery: HKVerifiableClinicalRecordCredentialType

A value that represents recovery information.

### Creating Record Types

init(rawValue: String)

Creates a record type based on the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Clinical record queries

struct HKVerifiableClinicalRecordQueryDescriptor

A query interface that provides one-time access to a SMART Health Card or EU Digital COVID Certificate using Swift concurrency.

class HKVerifiableClinicalRecordQuery

A query for one-time access to a SMART Health Card or EU Digital COVID Certificate.

struct HKVerifiableClinicalRecordSourceType

The source type for the verifiable clinical record.

class HKDocumentQuery

A query that returns a snapshot of all matching documents currently saved in the HealthKit store.

