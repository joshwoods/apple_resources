

- UIKit
- UITargetedPreview
-  retargetedPreview(with:) 

Instance Method

# retargetedPreview(with:)

Returns a targeted preview object with the same view and parameters, but with a different target container.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func retargetedPreview(with newTarget: UIPreviewTarget) -> UITargetedPreview
```

## Parameters 

`newTarget`  

The new target for the existing view.

## Return Value

A new targeted preview object containing the specified target and the current view.

