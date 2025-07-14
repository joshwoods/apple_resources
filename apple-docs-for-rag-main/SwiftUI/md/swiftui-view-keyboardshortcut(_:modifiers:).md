

- SwiftUI
- View
-  keyboardShortcut(\_:modifiers:) 

Instance Method

# keyboardShortcut(\_:modifiers:)

Defines a keyboard shortcut and assigns it to the modified control.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
nonisolated
func keyboardShortcut(
    _ key: KeyEquivalent,
    modifiers: EventModifiers = .command
) -> some View
```

## Discussion

Pressing the control’s shortcut while the control is anywhere in the frontmost window or scene, or anywhere in the macOS main menu, is equivalent to direct interaction with the control to perform its primary action.

The target of a keyboard shortcut is resolved in a leading-to-trailing, depth-first traversal of one or more view hierarchies. On macOS, the system looks in the key window first, then the main window, and then the command groups; on other platforms, the system looks in the active scene, and then the command groups.

If multiple controls are associated with the same shortcut, the first one found is used.

The default localization configuration is set to automatic.

## See Also

### Creating keyboard shortcuts

func keyboardShortcut(_:)

Assigns a keyboard shortcut to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

var keyboardShortcut: KeyboardShortcut?

The keyboard shortcut that buttons in this environment will be triggered with.

struct KeyboardShortcut

Keyboard shortcuts describe combinations of keys on a keyboard that the user can press in order to activate a button or toggle.

struct KeyEquivalent

Key equivalents consist of a letter, punctuation, or function key that can be combined with an optional set of modifier keys to specify a keyboard shortcut.

struct EventModifiers

A set of key modifiers that you can add to a gesture.

