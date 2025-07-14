

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:configuration:dismissalPreviewForItemWithIdentifier:) 

Instance Method

# contextMenuInteraction(\_:configuration:dismissalPreviewForItemWithIdentifier:)

Asks the delegate for a preview of the item with the specified identifier when a context-menu interaction ends.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    configuration: UIContextMenuConfiguration,
    dismissalPreviewForItemWithIdentifier identifier: any NSCopying
) -> UITargetedPreview?
```

## Parameters 

`interaction`  

The context-menu interaction object.

`configuration`  

The configuration of the menu to dismiss.

`identifier`  

The identifier for the item to generate a preview for.

## Return Value

A targeted preview object corresponding to the item with the identifier to use during the menu’s dismissal animation.

## Discussion

The system calls this method when a context-menu dismissal occurs. Implement this method to override the default dismissal preview that the system generates for the item.

## See Also

### Customizing the preview animations

func contextMenuInteraction(UIContextMenuInteraction, configuration: UIContextMenuConfiguration, highlightPreviewForItemWithIdentifier: any NSCopying) -> UITargetedPreview?

Asks the delegate for a preview of the item with the specified identifier when a context-menu interaction begins.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

