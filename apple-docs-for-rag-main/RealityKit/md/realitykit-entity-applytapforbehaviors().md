

- RealityKit
- Entity
-  applyTapForBehaviors() 

Instance Method

# applyTapForBehaviors()

Apply a tap to an Entity or one of its ancestors to trigger a RealityComposer behavior if one is present.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func applyTapForBehaviors() -> Bool
```

## Return Value

`true` if a tap trigger was fired, otherwise returns `false`.

## Discussion

This method looks for a RealityComposer tap trigger, starting with `self` and moving up the Entity hierarchy. As soon as an entity with a tap trigger is found, the trigger is fired, and the method returns `true`. If no tap trigger is found, the method returns `false`.

```
struct ContentView: View {
  var body: some View {
    RealityView() { content in
      if let entity = try? await Entity(named: "Content") {
        content.add(entity)
      }
    }.gesture(TapGesture().targetedToAnyEntity().onEnded { value in
      if value.entity.applyTapForBehaviors() {
        // Behavior was activated
      } else {
        // Behavior was not activated
      }
    })
  }
}
```

