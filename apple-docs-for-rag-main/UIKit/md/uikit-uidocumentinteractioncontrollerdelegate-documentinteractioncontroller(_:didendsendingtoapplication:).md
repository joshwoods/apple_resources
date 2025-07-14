

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionController(\_:didEndSendingToApplication:) 

Instance Method

# documentInteractionController(\_:didEndSendingToApplication:)

Called when a document interaction controller’s document has been handed off to the specified application.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentInteractionController(
    _ controller: UIDocumentInteractionController,
    didEndSendingToApplication application: String?
)
```

## Parameters 

`controller`  

The document interaction controller whose document is about to be opened.

`application`  

The bundle identifier of the application that is about to open the document. This value corresponds to the value in the `CFBundleIdentifier` key of the application’s `Info.plist` file.

## Discussion

This method is called after the document information has been saved for the specified application.

## See Also

### Opening files

func documentInteractionController(UIDocumentInteractionController, willBeginSendingToApplication: String?)

Called when a document interaction controller’s document is about to be opened by the specified application.

