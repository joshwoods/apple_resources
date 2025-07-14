

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerDidEndPreview(\_:) 

Instance Method

# documentInteractionControllerDidEndPreview(\_:)

Called when a document interaction controller has dismissed its document preview.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerDidEndPreview(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that dismissed its document preview.

## Discussion

This method is called after the view containing the document preview has been removed from the application’s key window. You can use this notification to remove any interface elements you set up behind the preview elements.

## See Also

### Presenting the user interface

func documentInteractionControllerWillBeginPreview(UIDocumentInteractionController)

Called when a document interaction controller is about to display a preview for its document.

func documentInteractionControllerWillPresentOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an options menu.

func documentInteractionControllerDidDismissOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its options menu.

func documentInteractionControllerWillPresentOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an Open In menu.

func documentInteractionControllerDidDismissOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its Open In menu.

