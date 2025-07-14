

- UIKit
- UIPencilPreferredAction
-  UIPencilPreferredAction.ignore 

Case

# UIPencilPreferredAction.ignore

An action that does nothing.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
case ignore
```

## Discussion

The system returns this action if any of the following conditions are true:

- The Apple Pencil doesn’t have a configured preferred action.

- The iPad’s accessibility settings disable Apple Pencil interactions.

## See Also

### Preferred actions

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

