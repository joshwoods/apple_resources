

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  database 

Instance Property

# database

The associated database.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var database: CKDatabase
```

## Discussion

Multiple sync engines can run in the same process, each targeting a different database. For example, you may use one sync engine for a person’s private database and another for their shared database.

Important

When using CloudKit’s production environment, don’t create multiple sync engines that target the same database. You can, however, do this in the development environment to help testing — for example, to simulate multiple devices syncing back and forth.

## See Also

### Managing attributes

var automaticallySync: Bool

A Boolean value that determines whether the engine syncs automatically.

var subscriptionID: CKSubscription.ID?

The subscription identifier for the associated database.

var stateSerialization: CKSyncEngine.State.Serialization?

The sync engine’s serialized state.

