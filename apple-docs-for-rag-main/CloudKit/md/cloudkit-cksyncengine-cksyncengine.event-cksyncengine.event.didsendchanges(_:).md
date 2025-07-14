

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.didSendChanges(\_:) 

Case

# CKSyncEngine.Event.didSendChanges(\_:)

An event that indicates a finished send operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case didSendChanges(CKSyncEngine.Event.DidSendChanges)
```

## See Also

### Pending local changes

case willSendChanges(CKSyncEngine.Event.WillSendChanges)

An event indicating an imminent send of local changes.

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

struct DidSendChanges

A type that provides information about a finished send operation.

