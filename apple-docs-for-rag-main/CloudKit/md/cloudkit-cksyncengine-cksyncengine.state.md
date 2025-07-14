

- CloudKit
- CKSyncEngine
-  CKSyncEngine.State 

Class

# CKSyncEngine.State

An object that manages the sync engine’s state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final class State
```

## Overview

To reliably and consistently sync your app’s data, a sync engine keeps a record of several important pieces of data, such as server changes tokens (for databases and record zones), subscription identifiers, the most recent userRecordID, and so on. This class automatically manages that state on behalf of your app, but there are certain elements you can modify. For example, you control the list of pending changes to send to the iCloud servers and manipulate that list using the add(pendingDatabaseChanges:) and add(pendingRecordZoneChanges:) methods. If there aren’t any scheduled sync operations when you invoke these methods, the engine automatically schedules one.

An engine’s state changes periodically and, when it does, the sync engine dispatches a CKSyncEngine.Event.stateUpdate(_:) event to your delegate. The event contains an instance of CKSyncEngine.State.Serialization and, on receipt of such an event, it’s your responsibility to persist the serialized state to disk so that it’s available across app launches. On the next initialization of the sync engine, you provide the most recently persisted state as part of the engine’s configuration. For more information, see init(database:stateSerialization:delegate:).

## Topics

### Accessing pending changes

var hasPendingUntrackedChanges: Bool

A Boolean value that indicates whether there are pending changes that the sync engine is unaware of.

var pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange]

The database changes that the sync engine has yet to send to the iCloud servers.

var pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange]

The record zone changes that the sync engine has yet to send to the iCloud servers.

### Manipulating pending changes

func add(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Adds the specified database changes to the state.

func remove(pendingDatabaseChanges: [CKSyncEngine.PendingDatabaseChange])

Removes the specified database changes from the state.

enum PendingDatabaseChange

Describes an unsent database modification.

func add(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Adds the specified record zone changes to the state.

func remove(pendingRecordZoneChanges: [CKSyncEngine.PendingRecordZoneChange])

Removes the specified record zone changes from the state.

enum PendingRecordZoneChange

Describes an unsent record modification.

### Serializing state

struct Serialization

A type that contains the serialized representation of a sync engine’s state.

### Instance Properties

var zoneIDsWithUnfetchedServerChanges: [CKRecordZone.ID]

## Relationships

### Conforms To

- Sendable

## See Also

### Accessing the engine’s attributes

var database: CKDatabase

The associated database.

var state: CKSyncEngine.State

The sync engine’s state.

