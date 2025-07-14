

- RealityKit
- RealityViewDefaultPlaceholder
-  windowMinimizeBehavior(\_:) 

Instance Method

# windowMinimizeBehavior(\_:)

Configures the minimize functionality for the window enclosing `self`.

RealityKitSwiftUImacOS 15.0+

``` source
nonisolated
func windowMinimizeBehavior(_ behavior: WindowInteractionBehavior) -> some View
```

## Parameters 

`behavior`  

The resize behavior.

## Discussion

On macOS, windows which support being minimized will move into the Dock when the minimize button is clicked, or the corresponding menu item is selected.

By default, the window minimize functionality is determined by the scene, as well as any modifiers applied to it.

You can use this modifier to override the default behavior.

For example, you can create a custom “About” window which disables the minimize functionality:

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

