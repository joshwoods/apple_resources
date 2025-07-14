

- SwiftUI
- KeyboardShortcut
-  key 

Instance Property

# key

The key equivalent that the user presses in conjunction with any specified modifier keys to activate the shortcut.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var key: KeyEquivalent
```

## See Also

### Creating a shortcut

init(KeyEquivalent, modifiers: EventModifiers)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

var modifiers: EventModifiers

The modifier keys that the user presses in conjunction with a key equivalent to activate the shortcut.

