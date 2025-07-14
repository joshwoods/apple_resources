

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.SentDatabaseChanges 

Structure

# CKSyncEngine.Event.SentDatabaseChanges

A type that provides information about a sent batch of database changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct SentDatabaseChanges
```

## Topics

### Accessing successful changes

let deletedZoneIDs: [CKRecordZone.ID]

The unique identifiers of the deleted record zones.

let savedZones: [CKRecordZone]

The modified record zones.

### Accessing failed changes

let failedZoneDeletes: [CKRecordZone.ID : CKError]

The unique identifiers of the record zones CloudKit is unable to delete, and the reasons why.

let failedZoneSaves: [CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave]

The record zones that CloudKit is unable to modify.

struct FailedZoneSave

A type that describes an unsuccessful attempt to modify a single record zone.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Pending local changes

case willSendChanges(CKSyncEngine.Event.WillSendChanges)

An event indicating an imminent send of local changes.

struct WillSendChanges

A type that provides information about an imminent send of local changes.

case sentDatabaseChanges(CKSyncEngine.Event.SentDatabaseChanges)

An event indicating a sent batch of database changes.

case sentRecordZoneChanges(CKSyncEngine.Event.SentRecordZoneChanges)

An event indicating a sent batch of record zone changes.

struct SentRecordZoneChanges

A type that provides information about a sent batch of record zone changes.

case didSendChanges(CKSyncEngine.Event.DidSendChanges)

An event that indicates a finished send operation.

struct DidSendChanges

A type that provides information about a finished send operation.

