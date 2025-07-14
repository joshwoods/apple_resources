

- BrowserEngineKit
- BETextInteraction
-  contextMenuInteractionDelegate 

Instance Property

# contextMenuInteractionDelegate

The delegate for the context menu interaction associated with this text interaction.

iOS 17.4+iPadOS 17.4+visionOS 1.1+

``` source
@MainActor
weak var contextMenuInteractionDelegate: (any UIContextMenuInteractionDelegate)? { get set }
```

## Overview

Set this object to receive delegate callbacks from the contextMenuInteraction.

## See Also

### Menus

func presentEditMenuForSelection()

Presents an edit menu for the current text selection.

func dismissEditMenuForSelection()

Dismisses the edit menu for the current text selection.

var contextMenuInteraction: UIContextMenuInteraction

An interaction you use to work with the text view’s context menu.

