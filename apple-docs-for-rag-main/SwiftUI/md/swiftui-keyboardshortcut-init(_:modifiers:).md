

- SwiftUI
- KeyboardShortcut
-  init(\_:modifiers:) 

Initializer

# init(\_:modifiers:)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    _ key: KeyEquivalent,
    modifiers: EventModifiers = .command
)
```

## Discussion

The localization configuration defaults to automatic.

## See Also

### Creating a shortcut

var key: KeyEquivalent

The key equivalent that the user presses in conjunction with any specified modifier keys to activate the shortcut.

var modifiers: EventModifiers

The modifier keys that the user presses in conjunction with a key equivalent to activate the shortcut.

