

- SwiftUI
- KeyboardShortcut
-  defaultAction 

Type Property

# defaultAction

The standard keyboard shortcut for the default button, consisting of the Return (↩) key and no modifiers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static let defaultAction: KeyboardShortcut
```

## Discussion

On macOS, the default button is designated with special coloration. If more than one control is assigned this shortcut, only the first one is emphasized.

## See Also

### Getting standard shortcuts

static let cancelAction: KeyboardShortcut

The standard keyboard shortcut for cancelling the in-progress action or dismissing a prompt, consisting of the Escape (⎋) key and no modifiers.

