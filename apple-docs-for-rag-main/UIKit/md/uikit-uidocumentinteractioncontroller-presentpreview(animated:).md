

- UIKit
- UIDocumentInteractionController
-  presentPreview(animated:) 

Instance Method

# presentPreview(animated:)

Displays a full-screen preview of the target document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func presentPreview(animated: Bool) -> Bool
```

## Parameters 

`animated`  

Specify true to animate the appearance of the document preview or false to display it immediately.

## Return Value

true if this method was able to display the document preview or false if it was not.

## Discussion

To use this method, you must first provide a delegate object that implements the documentInteractionControllerViewControllerForPreview(_:) method. The view controller returned by that method is used to present the document preview modally.

If your delegate implements the documentInteractionControllerViewForPreview(_:) and documentInteractionControllerRectForPreview(_:) methods, the view and rectangle returned by those methods is used as the starting point for the animation used to display the document preview. If the animated parameter is true but your delegate does not implement the documentInteractionControllerViewForPreview(_:) method (or that method returns `nil`), the document preview is animated into place using a crossfade transition.

This method displays the document preview asynchronously. The document interaction controller dismisses the document preview automatically in response to appropriate user interactions. You can also dismiss the preview programmatically using the dismissPreview(animated:) method.

## See Also

### Presenting and dismissing a document preview

func dismissPreview(animated: Bool)

Dismisses the currently active document preview.

