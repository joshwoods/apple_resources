

- RealityKit
- FromToByAction
-  subscribe(to:\_:) 

Type Method

# subscribe(to:\_:)

Subscribes to a serializable action event.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func subscribe(
    to eventType: ActionEventType,
    _ handler: @escaping @MainActor (ActionEvent) -> Void
)
```

Available when `Self` conforms to `Decodable`, `Self` conforms to `Encodable`, `EventParameterType` conforms to `Decodable`, and `EventParameterType` conforms to `Encodable`.

## Discussion

For example, you can call this method to subscribe to the update event, which the system calls each frame it evaluates the action:

```
struct MyAction: EntityAction {
    ...
}
MyAction.subscribe(to: .updated) { event in
    // RealityKit calls this closure in lock step as it
    // processes each animation frame.
}
```

