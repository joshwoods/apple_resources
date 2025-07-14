

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerWillPresentOpenInMenu(\_:) 

Instance Method

# documentInteractionControllerWillPresentOpenInMenu(\_:)

Called when a document interaction controller is about to display an Open In menu.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerWillPresentOpenInMenu(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that is about to display a menu.

## Discussion

The Open In menu is used to select an application for opening the current file. You can use this method to update your user interface in response to displaying the menu.

## See Also

### Presenting the user interface

func documentInteractionControllerWillBeginPreview(UIDocumentInteractionController)

Called when a document interaction controller is about to display a preview for its document.

func documentInteractionControllerDidEndPreview(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its document preview.

func documentInteractionControllerWillPresentOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an options menu.

func documentInteractionControllerDidDismissOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its options menu.

func documentInteractionControllerDidDismissOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its Open In menu.

