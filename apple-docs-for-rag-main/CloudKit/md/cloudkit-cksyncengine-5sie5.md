

- CloudKit
-  CKSyncEngine 

Class

# CKSyncEngine

An object that manages the synchronization of local and remote record data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final class CKSyncEngine
```

## Mentioned in 

Deciding whether CloudKit is right for your app

## Overview

Use CKSyncEngine to handle your app’s CloudKit sync operations and benefit from the performance and reliability it provides. To use the class, create an instance early in your app’s launch process and specify a database to sync. Thereafter, and depending on good system conditions, the sync engine will periodically push and pull database and record zone changes on the app’s behalf. To participate in those sync operations and to provide the engine with the changes to send, create a type that conforms to CKSyncEngineDelegate and assign an instance of it to the engine’s configuration. You can have multiple instances of CKSyncEngine in a single process, each targeting a different database. For example, you may have one syncing a person’s private database and another syncing their shared database.

Because periodic sync relies on good system conditions — adequate battery charge, an active network connection, a signed-in iCloud account, and so on — the engine’s sync schedule is indeterminate; if you need to sync immediately, like when you need to ensure your app has the most recent changes before continuing, use the fetchChanges(_:) and sendChanges(_:) methods.

The sync engine uses an opaque type to track its internal state, and it’s your responsibility to persist that state to disk and make it available across app launches so the engine can function properly. For more information, see handleEvent(_:syncEngine:) and CKSyncEngine.Event.StateUpdate.

CKSyncEngine requires the CloudKit and Remote notifications entitlements. For more information, see Configuring iCloud services and Configuring background execution modes.

Important

Don’t use CKSyncEngine to sync your app’s public database.

### Send changes to iCloud

A sync engine requires you to tell it about any changes to send, which you do by invoking the add(pendingDatabaseChanges:) and add(pendingRecordZoneChanges:) methods on the engine’s state property. If there are no scheduled sync operations when you invoke these methods, the engine automatically schedules one. Database changes don’t require any additional input, but the sync engine does expect you to provide the individual record zone changes — in batches — and return them from your delegate’s implementation of nextRecordZoneChangeBatch(_:syncEngine:). After the engine sends the changes, it notifies your delegate about their success (or failure) by dispatching CKSyncEngine.Event.sentDatabaseChanges(_:) and CKSyncEngine.Event.sentRecordZoneChanges(_:) events.

### Fetch changes from iCloud

By default, a sync engine attempts to discover an existing CKDatabaseSubscription for the associated database and uses that to receive silent notifications about remote record changes. If the engine doesn’t find a subscription, it automatically creates one to use. On receipt of a notification, the engine schedules a sync operation to fetch the related changes. When that operation runs, the engine dispatches a CKSyncEngine.Event.willFetchChanges(_:) event to your delegate. As it receives fetched changes, the engine dispatches CKSyncEngine.Event.fetchedDatabaseChanges(_:) and CKSyncEngine.Event.fetchedRecordZoneChanges(_:), accordingly. After the operation finishes, the sync engine notifies your delegate by dispatching a CKSyncEngine.Event.didFetchChanges(_:) event. You handle all dispatched events in your delegate’s implementation of handleEvent(_:syncEngine:).

Tip

A sample code project for CKSyncEngine is available on GitHub here: CloudKit Samples: CKSyncEngine.

## Topics

### Creating a sync engine

init(CKSyncEngine.Configuration)

Creates a sync engine with the specified configuration.

struct Configuration

A type that configures the attributes and behavior of a sync engine.

### Accessing the engine’s attributes

var database: CKDatabase

The associated database.

var state: CKSyncEngine.State

The sync engine’s state.

class State

An object that manages the sync engine’s state.

### Participating in scheduled sync operations

protocol CKSyncEngineDelegate

An interface for providing record data to a sync engine and customizing that engine’s behavior.

### Invoking manual sync operations

func fetchChanges(CKSyncEngine.FetchChangesOptions) async throws

Fetches pending remote changes from the server.

struct FetchChangesOptions

A set of options to use with a fetch operation.

func sendChanges(CKSyncEngine.SendChangesOptions) async throws

Sends pending local changes to the server.

struct SendChangesOptions

A set of options to use with a send operation.

### Canceling operations

func cancelOperations() async

Cancels any in-progress or pending sync operations.

### Structures

struct FetchChangesContext

struct RecordZoneChangeBatch

A type that contains the record changes for a single send operation.

struct SendChangesContext

A type that describes a single attempt to send changes to the iCloud servers.

### Enumerations

enum Event

Describes an event that occurs during a sync operation.

enum PendingDatabaseChange

Describes an unsent database modification.

enum PendingRecordZoneChange

Describes an unsent record modification.

enum SyncReason

Describes the reason for a sync operation.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Records

Local Records

Manipulate records on-device and save changes to the server.

Remote Records

Use subscriptions and change tokens to efficiently manage modifications to remote records.

Shared Records

Share one or more records with other iCloud users.

