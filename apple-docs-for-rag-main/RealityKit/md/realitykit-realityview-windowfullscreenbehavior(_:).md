

- RealityKit
- RealityView
-  windowFullScreenBehavior(\_:) 

Instance Method

# windowFullScreenBehavior(\_:)

Configures the full screen functionality for the window enclosing `self`.

RealityKitSwiftUImacOS 15.0+

``` source
nonisolated
func windowFullScreenBehavior(_ behavior: WindowInteractionBehavior) -> some View
```

## Parameters 

`behavior`  

The full screen behavior.

## Discussion

By default, the window full screen functionality is determined by the scene, as well as any modifiers applied to it. Additionally, when using the `Scene/windowResizability(_:)` modifier, the maximum size of the window’s contents will also determine whether a window can be made full screen.

You can use this modifier to override the default behavior.

For example, you can specify that a window cannot enter full screen mode:

```
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
                .windowFullScreenBehavior(.disabled)
        }
    }
}
```

