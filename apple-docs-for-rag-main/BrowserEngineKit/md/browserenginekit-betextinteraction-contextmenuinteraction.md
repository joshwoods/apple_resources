

- BrowserEngineKit
- BETextInteraction
-  contextMenuInteraction 

Instance Property

# contextMenuInteraction

An interaction you use to work with the text view’s context menu.

iOS 17.4+iPadOS 17.4+visionOS 1.1+

``` source
@MainActor
var contextMenuInteraction: UIContextMenuInteraction { get }
```

## Overview

Set the context menu interaction’s delegate by supplying a value for contextMenuInteractionDelegate.

## See Also

### Menus

func presentEditMenuForSelection()

Presents an edit menu for the current text selection.

func dismissEditMenuForSelection()

Dismisses the edit menu for the current text selection.

var contextMenuInteractionDelegate: (any UIContextMenuInteractionDelegate)?

The delegate for the context menu interaction associated with this text interaction.

