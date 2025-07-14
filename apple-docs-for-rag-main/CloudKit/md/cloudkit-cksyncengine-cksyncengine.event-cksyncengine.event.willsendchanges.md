

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.WillSendChanges 

Structure

# CKSyncEngine.Event.WillSendChanges

A type that provides information about an imminent send of local changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct WillSendChanges
```

## Topics

### Accessing the context

let context: CKSyncEngine.SendChangesContext

The context of the imminent send request.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Pending local changes

case willSendChanges(CKSyncEngine.Event.WillSendChanges)

An event indicating an imminent send of local changes.

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

