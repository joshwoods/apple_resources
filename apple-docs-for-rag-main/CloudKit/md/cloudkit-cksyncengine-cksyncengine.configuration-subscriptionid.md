

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  subscriptionID 

Instance Property

# subscriptionID

The subscription identifier for the associated database.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var subscriptionID: CKSubscription.ID?
```

## Discussion

By default, a sync engine attempts to discover an existing subscription for the synced database. If one isn’t found, the engine creates an internal CKDatabaseSubscription and uses that to receive notifications about remote record changes.

If you require the sync engine to use a specific database subscription, assign that subscription’s identifier to this property. Doing so enables your app to be backwards compatible if you’re migrating to CKSyncEngine from a custom CloudKit sync implementation.

The default value is `nil`.

## See Also

### Managing attributes

var automaticallySync: Bool

A Boolean value that determines whether the engine syncs automatically.

var database: CKDatabase

The associated database.

var stateSerialization: CKSyncEngine.State.Serialization?

The sync engine’s serialized state.

