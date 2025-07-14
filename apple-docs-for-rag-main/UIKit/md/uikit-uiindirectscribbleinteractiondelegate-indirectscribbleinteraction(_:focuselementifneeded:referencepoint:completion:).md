

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:focusElementIfNeeded:referencePoint:completion:) 

Instance Method

# indirectScribbleInteraction(\_:focusElementIfNeeded:referencePoint:completion:)

Asks the delegate to focus an element to handle text edits.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    focusElementIfNeeded elementIdentifier: Self.ElementIdentifier,
    referencePoint focusReferencePoint: CGPoint,
    completion: @escaping ((any UIResponder & UITextInput)?) -> Void
)
```

**Required**

## Parameters 

`interaction`  

The interaction requesting to focus an element.

`elementIdentifier`  

The identifier of the element that should receive focus.

`focusReferencePoint`  

A CGPoint inside the element’s view.

`completion`  

A completion handler that you must call, either synchronously or asynchronously. On success, the first parameter should be the text input that became first responder and that handles text operations for this element. On failure, call the completion with a `nil` parameter.

## Return Value

In response to this callback, the implementation should make this element the currently focused one, and make the corresponding UITextInput become first responder.

If the element isn’t focused already, set the text selection to the character location closest to `focusReferencePoint` to avoid any scrolling or shifting of content.

If the element is already focused, make no changes to the selection. Before returning you must still call the completion handler with a reference to UITextInput.

## See Also

### Managing Focus

func indirectScribbleInteraction(any UIInteraction, isElementFocused: Self.ElementIdentifier) -> Bool

Asks the delegate if an element is currently focused, according to the internal state of the interaction’s view.

**Required**

func indirectScribbleInteraction(any UIInteraction, shouldDelayFocusForElement: Self.ElementIdentifier) -> Bool

Allow the delegate to delay focusing an element.

**Required** Default implementation provided.

