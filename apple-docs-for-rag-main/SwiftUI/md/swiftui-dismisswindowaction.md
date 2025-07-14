

- SwiftUI
-  DismissWindowAction 

Structure

# DismissWindowAction

An action that dismisses a window associated to a particular scene.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct DismissWindowAction
```

## Overview

Use the dismissWindow environment value to get the instance of this structure for a given Environment. Then call the instance to dismiss a window. You call the instance directly because it defines a callAsFunction(id:) method that Swift calls when you call the instance.

For example, you can define a button that closes an auxiliary window:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        #if os(macOS)
        Window("Auxiliary", id: "auxiliary") {
            AuxiliaryContentView()
        }
        #endif
    }
}

struct DismissWindowButton: View {
    @Environment(\.dismissWindow) private var dismissWindow

    var body: some View {
        Button("Close Auxiliary Window") {
            dismissWindow(id: "auxiliary")
        }
    }
}
```

If the window was opened with pushWindow, the original presenting will reappear when this action is performed.

## Topics

### Calling the action

func callAsFunction()

Dismisses the current window.

func callAsFunction(id: String)

Dismisses the window that’s associated with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D)

Dismisses the window defined by the window group that is presenting the specified value type and that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Dismisses the window defined by the window group that is presenting the specified value type.

## Relationships

### Conforms To

- Sendable

## See Also

### Closing windows

var dismissWindow: DismissWindowAction

A window dismissal action stored in a view’s environment.

var dismiss: DismissAction

An action that dismisses the current presentation.

struct DismissAction

An action that dismisses a presentation.

struct DismissBehavior

Programmatic window dismissal behaviors.

