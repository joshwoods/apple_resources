

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerWillPresentOptionsMenu(\_:) 

Instance Method

# documentInteractionControllerWillPresentOptionsMenu(\_:)

Called when a document interaction controller is about to display an options menu.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerWillPresentOptionsMenu(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that is about to display an options menu.

## Discussion

The options menu is used to present the user with options for previewing the document, opening it in an application, or copying its contents. You can use this method to update your user interface in response to displaying the menu.

## See Also

### Presenting the user interface

func documentInteractionControllerWillBeginPreview(UIDocumentInteractionController)

Called when a document interaction controller is about to display a preview for its document.

func documentInteractionControllerDidEndPreview(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its document preview.

func documentInteractionControllerDidDismissOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its options menu.

func documentInteractionControllerWillPresentOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an Open In menu.

func documentInteractionControllerDidDismissOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its Open In menu.

