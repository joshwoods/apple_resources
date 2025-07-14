

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  windowResizeBehavior(\_:) 

Instance Method

# windowResizeBehavior(\_:)

Configures the resize functionality for the window enclosing `self`.

RealityKitSwiftUImacOS 15.0+

``` source
nonisolated
func windowResizeBehavior(_ behavior: WindowInteractionBehavior) -> some View
```

## Parameters 

`behavior`  

The resize behavior.

## Discussion

By default, the window resizability functionality is determined by the scene, as well as any modifiers applied to it. Additionally, when using the `Scene/windowResizability(_:)` modifier, the minimum and maximum size of the window’s contents will also determine the resizability behavior.

You can use this modifier to override the default behavior.

For example, you can create a custom “About” window which only allows for dismissal:

```
struct MyApp: App {
    var body: some Scene {
        ...
        Window("About MyApp", id: "about") {
            AboutView()
                .windowResizeBehavior(.disabled)
                .windowMinimizeBehavior(.disabled)
        }
        .windowResizability(.contentSize)
    }
}
```

