

- SwiftUI
- KeyboardShortcut
-  init(\_:modifiers:localization:) 

Initializer

# init(\_:modifiers:localization:)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    _ key: KeyEquivalent,
    modifiers: EventModifiers = .command,
    localization: KeyboardShortcut.Localization
)
```

## Discussion

Use the `localization` parameter to specify a localization strategy for this shortcut.

## See Also

### Creating a localized shortcut

var localization: KeyboardShortcut.Localization

The localization strategy to apply to this shortcut.

struct Localization

Options for how a keyboard shortcut participates in automatic localization.

