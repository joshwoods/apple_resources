

- UIKit
- UIControl
-  menuAttachmentPoint(for:) 

Instance Method

# menuAttachmentPoint(for:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func menuAttachmentPoint(for configuration: UIContextMenuConfiguration) -> CGPoint
```

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

var contextMenuInteraction: UIContextMenuInteraction?

A context menu interaction for the control.

var isContextMenuInteractionEnabled: Bool

A Boolean value that determines whether the control enables its context menu interaction.

var showsMenuAsPrimaryAction: Bool

A Boolean value that determines whether the context menu interaction is the control’s primary action.

func contextMenuInteraction(UIContextMenuInteraction, configurationForMenuAtLocation: CGPoint) -> UIContextMenuConfiguration?

func contextMenuInteraction(UIContextMenuInteraction, previewForDismissingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, previewForHighlightingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

