

- HealthKit
-  HKDocumentTypeIdentifier 

Structure

# HKDocumentTypeIdentifier

The identifiers for documents.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKDocumentTypeIdentifier
```

## Overview

To create an HKDocumentType instance, pass an HKDocumentTypeIdentifier value to the documentType(forIdentifier:) method.

For the complete list of quantity type identifiers, see Document Types.

## Topics

### Document Types

static let CDA: HKDocumentTypeIdentifier

The CDA Document type identifier, used when requesting permission to read or share CDA documents.

### Initializers

init(rawValue: String)

Returns a newly initialized document type identifier using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating document types

class func documentType(forIdentifier: HKDocumentTypeIdentifier) -> HKDocumentType?

Returns the shared document type for the provided identifier.

