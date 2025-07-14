

- UIKit
- UIPreviewInteractionDelegate
-  previewInteractionShouldBegin(\_:) 

Instance Method

# previewInteractionShouldBegin(\_:)

Asks the delegate whether a preview interaction is allowed to begin.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func previewInteractionShouldBegin(_ previewInteraction: UIPreviewInteraction) -> Bool
```

## Parameters 

`previewInteraction`  

The preview interaction that’s responding to user input.

## Return Value

true if the preview interaction should continue into the preview and commit phases; otherwise false.

## Discussion

If you don’t implement this optional method, the default return value of true is assumed.

When false, no further delegate calls are made for the specified preview interaction until the user restarts the 3D Touch interaction.

## See Also

### Managing preview interactions

func previewInteraction(UIPreviewInteraction, didUpdatePreviewTransition: CGFloat, ended: Bool)

Informs the delegate of the progress through the preview phase of the preview interaction.

**Required**

func previewInteraction(UIPreviewInteraction, didUpdateCommitTransition: CGFloat, ended: Bool)

Informs the delegate of the preview interaction’s progress through the commit phase.

func previewInteractionDidCancel(UIPreviewInteraction)

Informs the delegate that the specified preview interaction was canceled.

**Required**

