

- CloudKit
- CKDatabase
- CKDatabase.DatabaseChange
-  CKDatabase.DatabaseChange.Deletion 

Structure

# CKDatabase.DatabaseChange.Deletion

A database change that represents the deletion of a record zone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct Deletion
```

## Topics

### Identifying the Deleted Record Zone

var zoneID: CKRecordZone.ID

The identifier of the deleted record zone.

var purged: Bool

A Boolean value that indicates whether the user deleted the record zone when managing their iCloud storage.

Deprecated

### Instance Properties

var reason: CKDatabase.DatabaseChange.Deletion.Reason

### Enumerations

enum Reason

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

