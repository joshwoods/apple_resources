

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionController(\_:performAction:) Deprecated

Instance Method

# documentInteractionController(\_:performAction:)

Called when a document interaction controller wants its delegate to perform a specified action with the associated document.

visionOS 1.0–1.0Deprecated

``` source
optional func documentInteractionController(
    _ controller: UIDocumentInteractionController,
    performAction action: Selector?
) -> Bool
```

Deprecated

Apps should use UIActivityViewController for actions.

## Parameters 

`controller`  

The document interaction controller managing an associated document.

`action`  

The selector representing the action to perform. You can invoke this selector directly on the object responsible for performing the action or use it to call the appropriate method.

## Return Value

true if the action was performed successfully or false if it was not.

## Discussion

The supported `action` selectors for this method are `copy:` and `print:`. (The `print:` selector is available in iOS 4.2 and later. Printing is supported only on devices that support multitasking.)

To implement a `copy:` action, write the contents of the document—directly, or modified according to the intent of your app—to the pasteboard.

To implement a `print:` action, use the shared print interaction controller object. Assign the url property of the document interaction controller to the print interaction controller’s printingItem property. Then present the printing user interface. For details, refer to UIPrintInteractionController and to Printing in Drawing and Printing Guide for iOS.

Instead of implementing printing code in this method, you can rely on the built-in printing support of the Quick Look framework. For document types that can be previewed, the options menu of a document interaction controller always contains a Quick Look item. If the user chooses that item, the resulting Quick Look view includes an action button in the navigation bar that, when tapped, offers a Print button. In this case, the system automatically handles printing. For details, refer to QLPreviewController and to Using the Quick Look Framework in Document Interaction Programming Topics for iOS.

## See Also

### Deprecated

func documentInteractionController(UIDocumentInteractionController, canPerformAction: Selector?) -> Bool

Called when a document interaction controller needs to know whether the specified action can be performed on the associated document.

Deprecated

