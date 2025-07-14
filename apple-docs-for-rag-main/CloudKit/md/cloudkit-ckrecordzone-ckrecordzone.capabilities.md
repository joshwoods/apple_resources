

- CloudKit
- CKRecordZone
-  CKRecordZone.Capabilities 

Structure

# CKRecordZone.Capabilities

The capabilities that a record zone supports.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
struct Capabilities
```

## Topics

### Creating Zone Capabilities

init(rawValue: UInt)

Creates a set of capabilities for a record zone.

### Zone Capabilities

static var atomic: CKRecordZone.Capabilities

A capability that allows atomic changes of multiple records.

static var fetchChanges: CKRecordZone.Capabilities

A capability for fetching only the changed records from a zone.

static var sharing: CKRecordZone.Capabilities

A capability for sharing a specific hierarchy of records.

static var zoneWideSharing: CKRecordZone.Capabilities

A capability for sharing the entire contents of a record zone.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the Zone Attributes

var zoneID: CKRecordZone.ID

The unique ID of the zone.

var capabilities: CKRecordZone.Capabilities

The capabilities that the zone supports.

