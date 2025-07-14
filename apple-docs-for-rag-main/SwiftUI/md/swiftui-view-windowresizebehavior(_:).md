

- SwiftUI
- View
-  windowResizeBehavior(\_:) 

Instance Method

# windowResizeBehavior(\_:)

Configures the resize functionality for the window enclosing `self`.

macOS 15.0+

``` source
nonisolated
func windowResizeBehavior(_ behavior: WindowInteractionBehavior) -> some View
```

## Parameters 

`behavior`  

The resize behavior.

## Discussion

By default, the window resizability functionality is determined by the scene, as well as any modifiers applied to it. Additionally, when using the windowResizability(_:) modifier, the minimum and maximum size of the window’s contents will also determine the resizability behavior.

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

## See Also

### Managing window behavior

struct WindowManagerRole

Options for defining how a scene’s windows behave when used within a managed window context, such as full screen mode and Stage Manager.

func windowManagerRole(WindowManagerRole) -> some Scene

Configures the role for windows derived from `self` when participating in a managed window context, such as full screen or Stage Manager.

struct WindowInteractionBehavior

Options for enabling and disabling window interaction behaviors.

func windowDismissBehavior(WindowInteractionBehavior) -> some View

Configures the dismiss functionality for the window enclosing `self`.

func windowFullScreenBehavior(WindowInteractionBehavior) -> some View

Configures the full screen functionality for the window enclosing `self`.

func windowMinimizeBehavior(WindowInteractionBehavior) -> some View

Configures the minimize functionality for the window enclosing `self`.

func windowBackgroundDragBehavior(WindowInteractionBehavior) -> some Scene

Configures the behavior of dragging a window by its background.

