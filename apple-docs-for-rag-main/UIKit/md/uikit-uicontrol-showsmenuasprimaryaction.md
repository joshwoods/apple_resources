

- UIKit
- UIControl
-  showsMenuAsPrimaryAction 

Instance Property

# showsMenuAsPrimaryAction

A Boolean value that determines whether the context menu interaction is the control’s primary action.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var showsMenuAsPrimaryAction: Bool { get set }
```

## Discussion

If this value is true, the contextMenuInteraction becomes the primary action of the control, and the menu shows in response to the touchDown event.

The default value is false.

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

var contextMenuInteraction: UIContextMenuInteraction?

A context menu interaction for the control.

var isContextMenuInteractionEnabled: Bool

A Boolean value that determines whether the control enables its context menu interaction.

func contextMenuInteraction(UIContextMenuInteraction, configurationForMenuAtLocation: CGPoint) -> UIContextMenuConfiguration?

func contextMenuInteraction(UIContextMenuInteraction, previewForDismissingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, previewForHighlightingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

func menuAttachmentPoint(for: UIContextMenuConfiguration) -> CGPoint

