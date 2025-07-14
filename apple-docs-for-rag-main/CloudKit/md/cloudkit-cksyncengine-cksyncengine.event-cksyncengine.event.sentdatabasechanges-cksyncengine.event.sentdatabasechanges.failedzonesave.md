

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentDatabaseChanges
-  CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave 

Structure

# CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave

A type that describes an unsuccessful attempt to modify a single record zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct FailedZoneSave
```

## Topics

### Accessing the record zone

let zone: CKRecordZone

The record zone that CloudKit is unable to modify.

### Accessing the error

let error: CKError

A error that describes the reason for the unsuccessful attempt to modify the associated record zone.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Accessing failed changes

let failedZoneDeletes: [CKRecordZone.ID : CKError]

The unique identifiers of the record zones CloudKit is unable to delete, and the reasons why.

let failedZoneSaves: [CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave]

The record zones that CloudKit is unable to modify.

