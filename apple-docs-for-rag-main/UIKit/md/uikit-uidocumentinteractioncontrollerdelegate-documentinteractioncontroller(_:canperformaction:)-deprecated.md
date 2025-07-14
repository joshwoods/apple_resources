

- UIKit
- UIDocumentInteractionControllerDelegate
-  documentInteractionController(\_:canPerformAction:) Deprecated

Instance Method

# documentInteractionController(\_:canPerformAction:)

Called when a document interaction controller needs to know whether the specified action can be performed on the associated document.

visionOS 1.0–1.0Deprecated

``` source
optional func documentInteractionController(
    _ controller: UIDocumentInteractionController,
    canPerformAction action: Selector?
) -> Bool
```

Deprecated

Apps should use UIActivityViewController for actions.

## Parameters 

`controller`  

The document interaction controller managing an associated document.

`action`  

The selector representing the action in question.

## Return Value

true if the specified action is supported for the associated document or false if it is not. If you do not implement this method, the return value is assumed to be false.

## Discussion

When building the options menu (invoked, for example, by the user performing a long press gesture), a document interaction controller calls this method to find out if your app can perform various actions. If you implement this method for a given action, you must also implement the documentInteractionController(_:performAction:) method for that action.

The supported `action` selectors for this method are `copy:` and `print:`. (The `print:` selector is available in iOS 4.2 and later. Printing is supported only on devices that support multitasking.)

For each action that you implement in the documentInteractionController(_:performAction:) delegate method, return true from this method if that action is available for the document.

## See Also

### Deprecated

func documentInteractionController(UIDocumentInteractionController, performAction: Selector?) -> Bool

Called when a document interaction controller wants its delegate to perform a specified action with the associated document.

Deprecated

