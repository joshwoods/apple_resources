

- CloudKit
- CKSyncEngineDelegate
-  handleEvent(\_:syncEngine:) 

Instance Method

# handleEvent(\_:syncEngine:)

Tells the delegate to handle the specified sync event.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func handleEvent(
    _ event: CKSyncEngine.Event,
    syncEngine: CKSyncEngine
) async
```

**Required**

## Parameters 

`event`  

Information about the event. An event may occur for a number of reasons, such as when new data is available or when the device’s iCloud account changes. For more information, see CKSyncEngine.Event.

`syncEngine`  

The sync engine that generates the event.

## Discussion

Important

On receipt of a CKSyncEngine.Event.stateUpdate(_:) event, you must persist the attached state to disk alongside your app data. The sync engine requires you to provide it with the most recent serialized state at initialization, and it’s your responsibility to make sure this is available across app launches.

The sync engines provides events serially; your delegate won’t receive the subsequent event until it finishes processing the current one and returns from this method.

## See Also

### Handling sync events

enum Event

Describes an event that occurs during a sync operation.

enum CKSyncEngineEventType

Describes an event that occurs during a sync operation.

