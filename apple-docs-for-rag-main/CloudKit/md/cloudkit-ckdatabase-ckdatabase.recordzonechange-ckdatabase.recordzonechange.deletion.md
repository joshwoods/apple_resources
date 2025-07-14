

- CloudKit
- CKDatabase
- CKDatabase.RecordZoneChange
-  CKDatabase.RecordZoneChange.Deletion 

Structure

# CKDatabase.RecordZoneChange.Deletion

A record zone change that represents the deletion of a record.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct Deletion
```

## Topics

### Identifying the Deleted Record

var recordID: CKRecord.ID

The identifier of the deleted record.

var recordType: CKRecord.RecordType

The record type of the deleted record.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

