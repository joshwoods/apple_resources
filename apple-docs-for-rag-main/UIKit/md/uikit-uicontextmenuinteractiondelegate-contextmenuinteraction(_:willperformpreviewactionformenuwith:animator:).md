

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:willPerformPreviewActionForMenuWith:animator:) 

Instance Method

# contextMenuInteraction(\_:willPerformPreviewActionForMenuWith:animator:)

Informs the delegate when a preview action begins.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    willPerformPreviewActionForMenuWith configuration: UIContextMenuConfiguration,
    animator: any UIContextMenuInteractionCommitAnimating
)
```

## Parameters 

`interaction`  

The interaction object that triggered the interaction.

`configuration`  

The context menu configuration.

`animator`  

The animator to configure custom animations.

## See Also

### Responding to the menu’s appearance

protocol UIContextMenuInteractionCommitAnimating

Methods adopted by system-supplied animator objects when committing preview-related animations.

