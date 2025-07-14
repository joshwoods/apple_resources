

- UIKit
- UITargetedDragPreview
-  retargetedPreview(with:) 

Instance Method

# retargetedPreview(with:)

Returns a new targeted drag item preview based on an existing one, but with a new geometric target.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func retargetedPreview(with newTarget: UIDragPreviewTarget) -> UITargetedDragPreview
```

## Parameters 

`newTarget`  

A new drag item preview target.

## Return Value

A new targeted drag preview.

## Discussion

You can use this method in the drop interaction delegate’s implementation of the dropInteraction(_:previewForDropping:withDefault:) method to replace the current targeted drag item preview with a different one.

