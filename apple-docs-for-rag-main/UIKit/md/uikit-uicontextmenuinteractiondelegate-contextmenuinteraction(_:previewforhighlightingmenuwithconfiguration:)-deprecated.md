

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:previewForHighlightingMenuWithConfiguration:) Deprecated

Instance Method

# contextMenuInteraction(\_:previewForHighlightingMenuWithConfiguration:)

Returns the source view to use when animating the appearance of the preview interface.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    previewForHighlightingMenuWithConfiguration configuration: UIContextMenuConfiguration
) -> UITargetedPreview?
```

Deprecated

Use contextMenuInteraction(_:configuration:highlightPreviewForItemWithIdentifier:) instead.

## Parameters 

`interaction`  

The interaction object that triggered the preview.

`configuration`  

The configuration object associated with the current interaction.

## Return Value

An object containing the source view and configuration parameters for the animation.

## Discussion

UIKit calls this method before an interaction begins, to give you an opportunity to supply a custom source view for the presentation animations. If you didn’t provide a preview handler block in the `configuration` data, UIKit displays the specified view in the preview interface.

## See Also

### Deprecated

func contextMenuInteraction(UIContextMenuInteraction, previewForDismissingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view to use when animating the appearance of the preview interface.

Deprecated

