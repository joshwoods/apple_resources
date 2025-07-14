

- RealityKit
- Entity actions
- OrbitEntityAction
-  EntityAction Implementations 

API Collection

# EntityAction Implementations

## Topics

### Instance Properties

var isReversible: Bool

A Boolean value that determines whether the action reverses prior operations when playback is reverses.

### Type Methods

static func registerAction()

Registers the serializable action into the action-types registry.

static func registerAction()

Registers the action into the action-types registry.

static func subscribe(to: ActionEventType, (ActionEvent&lt;Self>) -> Void)

Subscribes to an action event.

static func subscribe(to: ActionEventType, (ActionEvent&lt;Self>) -> Void)

Subscribes to a serializable action event.

static func unsubscribe(from: ActionEventType)

Unsubscribes from an action event.

static func unsubscribeAll()

Unsubscribes from all action events.

