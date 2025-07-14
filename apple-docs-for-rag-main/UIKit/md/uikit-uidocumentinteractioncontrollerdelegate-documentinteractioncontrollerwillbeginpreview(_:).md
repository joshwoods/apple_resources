

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerWillBeginPreview(\_:) 

Instance Method

# documentInteractionControllerWillBeginPreview(\_:)

Called when a document interaction controller is about to display a preview for its document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerWillBeginPreview(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that is about to preview its document.

## Discussion

This method is called shortly before the view containing the document preview is presented modally. You can use this notification to set up any additional interface elements behind the preview elements.

## See Also

### Presenting the user interface

func documentInteractionControllerDidEndPreview(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its document preview.

func documentInteractionControllerWillPresentOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an options menu.

func documentInteractionControllerDidDismissOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its options menu.

func documentInteractionControllerWillPresentOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an Open In menu.

func documentInteractionControllerDidDismissOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its Open In menu.

