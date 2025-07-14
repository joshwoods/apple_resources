

- SwiftUI
- Scene
-  windowBackgroundDragBehavior(\_:) 

Instance Method

# windowBackgroundDragBehavior(\_:)

Configures the behavior of dragging a window by its background.

macOS 15.0+

``` source
nonisolated
func windowBackgroundDragBehavior(_ behavior: WindowInteractionBehavior) -> some Scene
```

## Parameters 

`behavior`  

The behavior of dragging the modified window by its background.

## Return Value

A scene configured with the specified behavior of dragging it by its background background.

## Discussion

By default, or when you apply the automatic behavior, the system will determine the best suitable behavior based on the configuration of the modified scene.

You can use this modifier to override the default behavior. For example, to always enable dragging a window by its background:

```
struct MyApp: App {
    var body: some Scene {
        Window("About MyApp", id: "about") {
            AboutView()
        }
        .windowBackgroundDragBehavior(.enabled)
    }
}
```

If you want to let your users drag your window by a specific view instead of (or in addition to) letting them drag it by its background, use WindowDragGesture.

Applying the enabled behavior is equivalent to adding a WindowDragGesture to the window’s background view.

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

func windowResizeBehavior(WindowInteractionBehavior) -> some View

Configures the resize functionality for the window enclosing `self`.

