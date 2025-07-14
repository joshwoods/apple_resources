

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.StateUpdate 

Structure

# CKSyncEngine.Event.StateUpdate

A type that provides information about an update to the sync engine’s state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct StateUpdate
```

## Topics

### Accessing the state

let stateSerialization: CKSyncEngine.State.Serialization

The current state of the sync engine.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### State updates

case stateUpdate(CKSyncEngine.Event.StateUpdate)

An event indicating an update to the sync engine’s state.

