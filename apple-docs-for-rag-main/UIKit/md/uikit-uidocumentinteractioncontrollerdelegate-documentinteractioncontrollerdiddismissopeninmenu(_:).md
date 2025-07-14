

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerDidDismissOpenInMenu(\_:) 

Instance Method

# documentInteractionControllerDidDismissOpenInMenu(\_:)

Called when a document interaction controller has dismissed its Open In menu.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerDidDismissOpenInMenu(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that dismissed its menu.

## Discussion

You can use this method to remove any additional views or content you placed underneath the Open In menu in your documentInteractionControllerWillPresentOpenInMenu(_:) method.

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

func documentInteractionControllerWillPresentOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an Open In menu.

