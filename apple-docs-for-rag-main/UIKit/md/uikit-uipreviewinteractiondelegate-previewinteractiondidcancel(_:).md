

- UIKit
- UIPreviewInteractionDelegate
-  previewInteractionDidCancel(\_:) 

Instance Method

# previewInteractionDidCancel(\_:)

Informs the delegate that the specified preview interaction was canceled.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func previewInteractionDidCancel(_ previewInteraction: UIPreviewInteraction)
```

**Required**

## Parameters 

`previewInteraction`  

The preview interaction associated with the current user input.

## Discussion

This method is called when the preview interaction is canceled, either programmatically through the cancel() method on UIPreviewInteraction, or by interrupting the preview interaction before the commit phase is complete.

## See Also

### Managing preview interactions

func previewInteractionShouldBegin(UIPreviewInteraction) -> Bool

Asks the delegate whether a preview interaction is allowed to begin.

func previewInteraction(UIPreviewInteraction, didUpdatePreviewTransition: CGFloat, ended: Bool)

Informs the delegate of the progress through the preview phase of the preview interaction.

**Required**

func previewInteraction(UIPreviewInteraction, didUpdateCommitTransition: CGFloat, ended: Bool)

Informs the delegate of the preview interaction’s progress through the commit phase.

