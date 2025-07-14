

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:previewForDismissingMenuWithConfiguration:) Deprecated

Instance Method

# contextMenuInteraction(\_:previewForDismissingMenuWithConfiguration:)

Returns the destination view to use when animating the appearance of the preview interface.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    previewForDismissingMenuWithConfiguration configuration: UIContextMenuConfiguration
) -> UITargetedPreview?
```

Deprecated

Use contextMenuInteraction(_:configuration:dismissalPreviewForItemWithIdentifier:) instead.

## Parameters 

`interaction`  

The interaction object that triggered the preview.

`configuration`  

The configuration object associated with the current interaction.

## Return Value

An object containing the destination view and configuration parameters for the animation.

## Discussion

When the user dismisses the preview interface, UIKit animates that interface to the view you specify in the returned UITargetedPreview object.

## See Also

### Deprecated

func contextMenuInteraction(UIContextMenuInteraction, previewForHighlightingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the source view to use when animating the appearance of the preview interface.

Deprecated

