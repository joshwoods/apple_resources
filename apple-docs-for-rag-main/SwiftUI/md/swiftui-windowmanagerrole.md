

- SwiftUI
-  WindowManagerRole 

Structure

# WindowManagerRole

Options for defining how a scene’s windows behave when used within a managed window context, such as full screen mode and Stage Manager.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct WindowManagerRole
```

## Overview

Use values of this type in conjunction with the windowManagerRole(_:) modifier to override the default system behavior.

For example, you can specify that a secondary `Window` scene should use the principal role for full screen and Stage Manager:

```
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        Window("Organizer", id: "organizer") {
            OrganizerView()
        }
        .windowManagerRole(.principal)
    }
}
```

## Topics

### Type Properties

static let associated: WindowManagerRole

The associated role. Windows derived from this scene can be shown alongside windows with a `.principal` role in either full screen or Stage Manager, but do not participate in those modes on their own.

static let automatic: WindowManagerRole

The automatic role. The type and configuration of the scene will be used to determine how its windows behave in full screen and Stage Manager.

static let principal: WindowManagerRole

The principal role. Windows derived from this scene will show in full screen, if enabled, or in Stage Manager.

## Relationships

### Conforms To

- Sendable

## See Also

### Managing window behavior

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

func windowBackgroundDragBehavior(WindowInteractionBehavior) -> some Scene

Configures the behavior of dragging a window by its background.

