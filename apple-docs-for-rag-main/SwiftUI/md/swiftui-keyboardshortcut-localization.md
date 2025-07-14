

- SwiftUI
- KeyboardShortcut
-  localization 

Instance Property

# localization

The localization strategy to apply to this shortcut.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var localization: KeyboardShortcut.Localization
```

## See Also

### Creating a localized shortcut

init(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

struct Localization

Options for how a keyboard shortcut participates in automatic localization.

