

- SwiftUI
- Scene
-  keyboardShortcut(\_:) 

Instance Method

# keyboardShortcut(\_:)

Defines a keyboard shortcut for opening new scene windows.

macOS 13.0+

``` source
nonisolated
func keyboardShortcut(_ shortcut: KeyboardShortcut?) -> some Scene
```

## Parameters 

`shortcut`  

The keyboard shortcut for presenting the scene, or `nil`.

## Return Value

A scene that can be presented with a keyboard shortcut.

## Discussion

A scene’s keyboard shortcut is bound to the command it adds for creating new windows (in the case of `WindowGroup` and `DocumentGroup`) or bringing a singleton window forward (in the case of `Window` and, on macOS, `Settings` and `UtilityWindow`). Pressing the keyboard shortcut is equivalent to selecting the menu command.

In cases where a command already has a keyboard shortcut, the scene’s keyboard shortcut is used instead. For example, `WindowGroup` normally creates a File \> New Window menu command whose keyboard shortcut is `⌘N`. The following code changes it to something based on dynamic state:

```
@main
struct Notes: App {
    @State private var newWindowShortcut: KeyboardShortcut? = ...

    var body: some Scene {
        WindowGroup {
            ContentView($newWindowShortcut)
        }
        .keyboardShortcut(newWindowShortcut)
    }
}
```

If `shortcut` is `nil`, the scene’s presentation command will not be associated with a keyboard shortcut, even if SwiftUI normally assigns one automatically.

## See Also

### Setting commands

func commands&lt;Content>(content: () -> Content) -> some Scene

Adds commands to the scene.

func commandsRemoved() -> some Scene

Removes all commands defined by the modified scene.

func commandsReplaced&lt;Content>(content: () -> Content) -> some Scene

Replaces all commands defined by the modified scene with the commands from the builder.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization) -> some Scene

Defines a keyboard shortcut for opening new scene windows.

