

- CloudKit
- CKSyncEngine
- CKSyncEngine.Configuration
-  stateSerialization 

Instance Property

# stateSerialization

The sync engine’s serialized state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var stateSerialization: CKSyncEngine.State.Serialization?
```

## Discussion

This property returns the value you specify for the initializer’s `stateSerialization` parameter. If you choose to set this property after initialization, assign the state from the most recent CKSyncEngine.Event.stateUpdate(_:) event handled by your delegate. However, If this is the first initialization of the associated sync engine, specify `nil` instead.

The default value is `nil`.

## See Also

### Managing attributes

var automaticallySync: Bool

A Boolean value that determines whether the engine syncs automatically.

var database: CKDatabase

The associated database.

var subscriptionID: CKSubscription.ID?

The subscription identifier for the associated database.

