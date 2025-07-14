

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.StateUpdate
-  stateSerialization 

Instance Property

# stateSerialization

The current state of the sync engine.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let stateSerialization: CKSyncEngine.State.Serialization
```

## Discussion

Important

Always persist the most recent state to disk alongside your app data. The sync engine requires you to provide it with the most recent serialized state at initialization, and it’s your responsibility to make sure the state is available across app launches.

