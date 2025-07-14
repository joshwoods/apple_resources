

- SwiftUI
- View
-  windowMinimizeBehavior(\_:) 

Instance Method

# windowMinimizeBehavior(\_:)

Configures the minimize functionality for the window enclosing `self`.

macOS 15.0+

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

func windowResizeBehavior(WindowInteractionBehavior) -> some View

Configures the resize functionality for the window enclosing `self`.

func windowBackgroundDragBehavior(WindowInteractionBehavior) -> some Scene

Configures the behavior of dragging a window by its background.

