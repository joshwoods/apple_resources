

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.willSendChanges(\_:) 

Case

# CKSyncEngine.Event.willSendChanges(\_:)

An event indicating an imminent send of local changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case willSendChanges(CKSyncEngine.Event.WillSendChanges)
```

## Discussion

A send operation may send all local changes, only changes to a specific set of records, or only those in a specific record zone. Use this case’s associated value to determine the scope for the current operation. For more information, see CKSyncEngine.SendChangesContext.

## See Also

### Pending local changes

struct WillSendChanges

A type that provides information about an imminent send of local changes.

case sentDatabaseChanges(CKSyncEngine.Event.SentDatabaseChanges)

An event indicating a sent batch of database changes.

struct SentDatabaseChanges

A type that provides information about a sent batch of database changes.

case sentRecordZoneChanges(CKSyncEngine.Event.SentRecordZoneChanges)

An event indicating a sent batch of record zone changes.

struct SentRecordZoneChanges

A type that provides information about a sent batch of record zone changes.

case didSendChanges(CKSyncEngine.Event.DidSendChanges)

An event that indicates a finished send operation.

struct DidSendChanges

A type that provides information about a finished send operation.

