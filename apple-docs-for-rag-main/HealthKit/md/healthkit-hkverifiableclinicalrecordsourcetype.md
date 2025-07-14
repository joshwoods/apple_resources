

- HealthKit
-  HKVerifiableClinicalRecordSourceType 

Structure

# HKVerifiableClinicalRecordSourceType

The source type for the verifiable clinical record.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+watchOS 8.5+

``` source
struct HKVerifiableClinicalRecordSourceType
```

## Topics

### Identifying Source Types

static let euDigitalCOVIDCertificate: HKVerifiableClinicalRecordSourceType

A value indicating EU Digital COVID Certificates.

static let smartHealthCard: HKVerifiableClinicalRecordSourceType

A value indicating SMART health cards.

### Creating Source Types

init(rawValue: String)

Creates a source type based on the provided string.

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

struct HKVerifiableClinicalRecordCredentialType

The type of record returned by a verifiable clinical record query.

class HKDocumentQuery

A query that returns a snapshot of all matching documents currently saved in the HealthKit store.

