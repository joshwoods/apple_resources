

- UIKit
-  UIPencilPreferredAction 

Enumeration

# UIPencilPreferredAction

The actions Apple Pencil can perform after a person performs a double tap or squeeze.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UIPencilPreferredAction
```

## Topics

### Preferred actions

case ignore

An action that does nothing.

case switchEraser

An action that switches between the current tool and the eraser.

case switchPrevious

An action that switches between the current tool and the last used tool.

case showColorPalette

An action that toggles the display of the color palette.

case showInkAttributes

An action that toggles the display of the selected tool’s ink attributes.

case showContextualPalette

An action that toggles shows a contextual palette of markup tools, or undo and redo options if tools aren’t available.

case runSystemShortcut

An action that runs a system shortcut.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining preferences for actions

class var preferredTapAction: UIPencilPreferredAction

A person’s preferred double-tap action for Apple Pencil, as specified in the Settings app.

class var preferredSqueezeAction: UIPencilPreferredAction

A person’s preferred squeeze action for Apple Pencil, as specified in the Settings app.

