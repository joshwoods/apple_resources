

- CloudKit
- CKSyncEngine
-  CKSyncEngine.Event 

Enumeration

# CKSyncEngine.Event

Describes an event that occurs during a sync operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum Event
```

## Overview

Important

You don’t create instances of this type manually. Instead, the sync engine provides them to your app’s delegate during sync operations.

## Topics

### Account changes

case accountChange(CKSyncEngine.Event.AccountChange)

An event indicating a change to the device’s iCloud account.

struct AccountChange

A type that provides information about a change to the device’s iCloud account.

### Remote database changes

case willFetchChanges(CKSyncEngine.Event.WillFetchChanges)

An event indicating an imminent database fetch.

struct WillFetchChanges

A type that provides information about an imminent database fetch.

case fetchedDatabaseChanges(CKSyncEngine.Event.FetchedDatabaseChanges)

An event indicating there are fetched database changes to process.

struct FetchedDatabaseChanges

A type that provides information about fetched database changes.

case didFetchChanges(CKSyncEngine.Event.DidFetchChanges)

An event that indicates the database fetch is done.

struct DidFetchChanges

A type that provides information about a finished database fetch.

### Remote record zone changes

case willFetchRecordZoneChanges(CKSyncEngine.Event.WillFetchRecordZoneChanges)

An event indicating an imminent fetch of changes in a record zone.

struct WillFetchRecordZoneChanges

A type that provides information about an imminent fetch of changes in a record zone.

case fetchedRecordZoneChanges(CKSyncEngine.Event.FetchedRecordZoneChanges)

An event indicating there are fetched record zone changes to process.

struct FetchedRecordZoneChanges

A type that provides information about fetched record zone changes.

case didFetchRecordZoneChanges(CKSyncEngine.Event.DidFetchRecordZoneChanges)

An event that indicates the record zone fetch is done.

struct DidFetchRecordZoneChanges

A type that provides information about a finished record zone fetch.

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

case didSendChanges(CKSyncEngine.Event.DidSendChanges)

An event that indicates a finished send operation.

struct DidSendChanges

A type that provides information about a finished send operation.

### State updates

case stateUpdate(CKSyncEngine.Event.StateUpdate)

An event indicating an update to the sync engine’s state.

struct StateUpdate

A type that provides information about an update to the sync engine’s state.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Handling sync events

func handleEvent(CKSyncEngine.Event, syncEngine: CKSyncEngine) async

Tells the delegate to handle the specified sync event.

**Required**

enum CKSyncEngineEventType

Describes an event that occurs during a sync operation.

