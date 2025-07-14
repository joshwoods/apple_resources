

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerViewForPreview(\_:) 

Instance Method

# documentInteractionControllerViewForPreview(\_:)

Called when a document interaction controller needs the starting point for animating the display of a document preview.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerViewForPreview(_ controller: UIDocumentInteractionController) -> UIView?
```

## Parameters 

`controller`  

The document interaction controller requesting the starting view.

## Return Value

The view to use as the starting point for the animation or `nil` if you want the document preview to fade into place.

## Discussion

By default, the starting rectangle for the animation is set to the bounds of the returned view. To specify a different starting rectangle, you must also override the documentInteractionControllerRectForPreview(_:) method.

## See Also

### Configuring the parent view controller

func documentInteractionControllerViewControllerForPreview(UIDocumentInteractionController) -> UIViewController

Called when a document interaction controller needs a view controller for presenting a document preview.

func documentInteractionControllerRectForPreview(UIDocumentInteractionController) -> CGRect

Called when a document interaction controller needs the rectangle to use as the starting point for animating the display of a document preview.

