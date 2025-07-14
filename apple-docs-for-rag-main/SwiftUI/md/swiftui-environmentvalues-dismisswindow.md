

- SwiftUI
- EnvironmentValues
-  dismissWindow 

Instance Property

# dismissWindow

A window dismissal action stored in a view’s environment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var dismissWindow: DismissWindowAction { get }
```

## Discussion

Use the `dismissWindow` environment value to get an DismissWindowAction instance for a given Environment. Then call the instance to dismiss a window. You call the instance directly because it defines a callAsFunction(id:) method that Swift calls when you call the instance.

For example, you can define a button that dismisses an auxiliary window:

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

If the window was opened with pushWindow, the presenting window will reappear when this action is performed.

## See Also

### Closing windows

struct DismissWindowAction

An action that dismisses a window associated to a particular scene.

var dismiss: DismissAction

An action that dismisses the current presentation.

struct DismissAction

An action that dismisses a presentation.

struct DismissBehavior

Programmatic window dismissal behaviors.

