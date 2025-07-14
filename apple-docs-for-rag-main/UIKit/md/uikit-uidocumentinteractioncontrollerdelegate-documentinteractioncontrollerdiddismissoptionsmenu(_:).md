

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionControllerDidDismissOptionsMenu(\_:) 

Instance Method

# documentInteractionControllerDidDismissOptionsMenu(\_:)

Called when a document interaction controller has dismissed its options menu.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionControllerDidDismissOptionsMenu(_ controller: UIDocumentInteractionController)
```

## Parameters 

`controller`  

The document interaction controller that dismissed its options menu.

## Discussion

You can use this method to remove any additional views or content you placed underneath the options menu in your documentInteractionControllerWillPresentOptionsMenu(_:) method.

## See Also

### Presenting the user interface

func documentInteractionControllerWillBeginPreview(UIDocumentInteractionController)

Called when a document interaction controller is about to display a preview for its document.

func documentInteractionControllerDidEndPreview(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its document preview.

func documentInteractionControllerWillPresentOptionsMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an options menu.

func documentInteractionControllerWillPresentOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller is about to display an Open In menu.

func documentInteractionControllerDidDismissOpenInMenu(UIDocumentInteractionController)

Called when a document interaction controller has dismissed its Open In menu.

