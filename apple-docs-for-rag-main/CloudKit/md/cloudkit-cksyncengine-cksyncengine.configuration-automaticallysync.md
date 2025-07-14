

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  automaticallySync 

Instance Property

# automaticallySync

A Boolean value that determines whether the engine syncs automatically.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var automaticallySync: Bool
```

## Discussion

By default, the sync engine uses the system scheduler to automatically schedule both send and fetch operations. If an operation fails due to a recoverable error, such as a network failure or when the server is enforcing request limits, the engine reschedules those operations as necessary. Unless you have a specific need, prefer to use the default behavior in your app.

If you set this property’s value to false, use fetchChanges(_:) and sendChanges(_:) to invoke immediate sync operations, allowing for more control over when your app syncs its records. For example, you may want to sync at a specific time of day or deterministically simulate certain conditions in your unit tests.

The default value is true.

## See Also

### Managing attributes

var database: CKDatabase

The associated database.

var subscriptionID: CKSubscription.ID?

The subscription identifier for the associated database.

var stateSerialization: CKSyncEngine.State.Serialization?

The sync engine’s serialized state.

