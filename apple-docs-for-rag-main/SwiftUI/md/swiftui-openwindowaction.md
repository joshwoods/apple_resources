

- SwiftUI
-  OpenWindowAction 

Structure

# OpenWindowAction

An action that presents a window.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct OpenWindowAction
```

## Overview

Use the openWindow environment value to get the instance of this structure for a given Environment. Then call the instance to open a window. You call the instance directly because it defines a callAsFunction(id:) method that Swift calls when you call the instance.

For example, you can define a button that opens a new mail viewer window:

```
@main
struct Mail: App {
    var body: some Scene {
        WindowGroup(id: "mail-viewer") {
            MailViewer()
        }
    }
}

struct NewViewerButton: View {
    @Environment(\.openWindow) private var openWindow

    var body: some View {
        Button("Open new mail viewer") {
            openWindow(id: "mail-viewer")
        }
    }
}
```

You indicate which scene to open by providing one of the following:

- A string identifier that you pass through the `id` parameter, as in the above example.

- A `value` parameter that has a type that matches the type that you specify in the scene’s initializer.

- Both an identifier and a value. This enables you to define multiple window groups that take input values of the same type, like a UUID.

Use the first option to target either a WindowGroup or a Window scene in your app that has a matching identifier. For a `WindowGroup`, the system creates a new window for the group. If the window group presents data, the system provides the default value or `nil` to the window’s root view. If the targeted scene is a `Window`, the system orders it to the front.

Use the other two options to target a `WindowGroup` and provide a value to present. If the interface already has a window from the group that’s presenting the specified value, the system brings the window to the front. Otherwise, the system creates a new window and passes a binding to the specified value.

## Topics

### Calling the action

func callAsFunction(id: String)

Opens a window that’s associated with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D)

Opens a window defined by the window group that presents the specified value type and that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Opens a window defined by a window group that presents the type of the specified value.

### Structures

struct SharingBehavior

### Instance Methods

func callAsFunction(id: String, sharingBehavior: OpenWindowAction.SharingBehavior) async throws

Opens a window that’s associated with the specified identifier, using the specified sharing sharingBehavior..

func callAsFunction&lt;D>(id: String, value: D, sharingBehavior: OpenWindowAction.SharingBehavior) async throws

Opens a window defined by the window group that presents the specified value type and that’s associated with the specified identifier, using the specified sharingBehavior.

func callAsFunction&lt;D>(value: D, sharingBehavior: OpenWindowAction.SharingBehavior) async throws

Opens a window defined by a window group that presents the type of the specified value, using the specified sharingBehavior.

## Relationships

### Conforms To

- Sendable

## See Also

### Opening windows

Presenting windows and spaces

Open and close the scenes that make up your app’s interface.

var supportsMultipleWindows: Bool

A Boolean value that indicates whether the current platform supports opening multiple windows.

var openWindow: OpenWindowAction

A window presentation action stored in a view’s environment.

struct PushWindowAction

An action that opens the requested window in place of the window the action is called from.

