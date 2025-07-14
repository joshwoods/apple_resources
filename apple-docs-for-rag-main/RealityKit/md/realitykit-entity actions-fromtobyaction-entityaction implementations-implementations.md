

- RealityKit
- Entity actions
- FromToByAction
-  EntityAction Implementations 

API Collection

# EntityAction Implementations

## Topics

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

