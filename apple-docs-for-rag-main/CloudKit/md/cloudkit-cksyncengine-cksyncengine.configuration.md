

- CloudKit
- CKSyncEngine
-  CKSyncEngine.Configuration 

Structure

# CKSyncEngine.Configuration

A type that configures the attributes and behavior of a sync engine.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct Configuration
```

## Topics

### Creating configurations

init(database: CKDatabase, stateSerialization: CKSyncEngine.State.Serialization?, delegate: any CKSyncEngineDelegate)

Creates a configuration for the specified database and serialized state.

### Handling record changes

var delegate: any CKSyncEngineDelegate

The object that provides the records to sync and handles any related events.

protocol CKSyncEngineDelegate

An interface for providing record data to a sync engine and customizing that engine’s behavior.

### Managing attributes

var automaticallySync: Bool

A Boolean value that determines whether the engine syncs automatically.

var database: CKDatabase

The associated database.

var subscriptionID: CKSubscription.ID?

The subscription identifier for the associated database.

var stateSerialization: CKSyncEngine.State.Serialization?

The sync engine’s serialized state.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Creating a sync engine

init(CKSyncEngine.Configuration)

Creates a sync engine with the specified configuration.

