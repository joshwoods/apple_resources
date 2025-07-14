

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerRectForPreview(\_:) 

Instance Method

# documentInteractionControllerRectForPreview(\_:)

Called when a document interaction controller needs the rectangle to use as the starting point for animating the display of a document preview.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerRectForPreview(_ controller: UIDocumentInteractionController) -> CGRect
```

## Parameters 

`controller`  

The document interaction controller requesting the starting rectangle.

## Return Value

A rectangle in the coordinate system of the view returned by the documentInteractionControllerViewForPreview(_:) method.

## Discussion

If you do not implement the documentInteractionControllerViewForPreview(_:) method, or if you do implement it but return a `nil` value, this method is not called. If you do not implement this method, the starting rectangle is assumed to be the bounds of the view returned by the documentInteractionControllerViewForPreview(_:) method.

## See Also

### Configuring the parent view controller

func documentInteractionControllerViewControllerForPreview(UIDocumentInteractionController) -> UIViewController

Called when a document interaction controller needs a view controller for presenting a document preview.

func documentInteractionControllerViewForPreview(UIDocumentInteractionController) -> UIView?

Called when a document interaction controller needs the starting point for animating the display of a document preview.

