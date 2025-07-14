

- SwiftUI
-  WindowInteractionBehavior 

Structure

# WindowInteractionBehavior

Options for enabling and disabling window interaction behaviors.

macOS 15.0+

``` source
struct WindowInteractionBehavior
```

## Overview

Use values of this type in conjunction with the following view and scene modifiers to adjust the supported functionality for the window:

- windowDismissBehavior(_:)

- windowMinimizeBehavior(_:)

- windowFullScreenBehavior(_:)

- windowResizeBehavior(_:)

- windowBackgroundDragBehavior(_:)

For example, you can create a custom “About” window which only allows for dismissal:

```
struct MyApp: App {
    var body: some Scene {
        ...
        Window("About MyApp", id: "about") {
            AboutView()
                .windowMinimizeBehavior(.disabled)
                .windowResizeBehavior(.disabled)
        }
        .windowResizability(.contentSize)
    }
}
```

## Topics

### Type Properties

static let automatic: WindowInteractionBehavior

The automatic behavior. The associated window behavior will be enabled or disabled depending on the configuration of the enclosing `Scene`.

static let disabled: WindowInteractionBehavior

The disabled behavior. The associated window interaction behavior will be disabled.

static let enabled: WindowInteractionBehavior

The enabled behavior. The associated window interaction behavior will be enabled.

## Relationships

### Conforms To

- Sendable

## See Also

### Managing window behavior

struct WindowManagerRole

Options for defining how a scene’s windows behave when used within a managed window context, such as full screen mode and Stage Manager.

func windowManagerRole(WindowManagerRole) -> some Scene

Configures the role for windows derived from `self` when participating in a managed window context, such as full screen or Stage Manager.

func windowDismissBehavior(WindowInteractionBehavior) -> some View

Configures the dismiss functionality for the window enclosing `self`.

func windowFullScreenBehavior(WindowInteractionBehavior) -> some View

Configures the full screen functionality for the window enclosing `self`.

func windowMinimizeBehavior(WindowInteractionBehavior) -> some View

Configures the minimize functionality for the window enclosing `self`.

func windowResizeBehavior(WindowInteractionBehavior) -> some View

Configures the resize functionality for the window enclosing `self`.

func windowBackgroundDragBehavior(WindowInteractionBehavior) -> some Scene

Configures the behavior of dragging a window by its background.

