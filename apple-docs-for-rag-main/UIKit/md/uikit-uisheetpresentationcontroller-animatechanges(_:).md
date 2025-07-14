

- UIKit
- UISheetPresentationController
-  animateChanges(\_:) 

Instance Method

# animateChanges(\_:)

Animates the UI changes to the sheet’s properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
func animateChanges(_ changes: () -> Void)
```

## Parameters 

`changes`  

A block where you change the sheet’s properties to animate them.

## Discussion

To animate changes to any of the sheet’s properties, set them inside the block that you pass to this method. By the time this method returns, layout finishes for the sheet, all adjacent sheets in the sheet stack, and their subviews.

