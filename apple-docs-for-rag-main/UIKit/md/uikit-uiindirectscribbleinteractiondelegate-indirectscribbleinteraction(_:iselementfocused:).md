

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:isElementFocused:) 

Instance Method

# indirectScribbleInteraction(\_:isElementFocused:)

Asks the delegate if an element is currently focused, according to the internal state of the interaction’s view.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    isElementFocused elementIdentifier: Self.ElementIdentifier
) -> Bool
```

**Required**

## Parameters 

`interaction`  

The interaction asking for the focused state.

`elementIdentifier`  

The identifier of the element the interaction is asking about.

## Return Value

Returns true if the element is the one currently focused.

## See Also

### Managing Focus

func indirectScribbleInteraction(any UIInteraction, focusElementIfNeeded: Self.ElementIdentifier, referencePoint: CGPoint, completion: ((any UIResponder &amp; UITextInput)?) -> Void)

Asks the delegate to focus an element to handle text edits.

**Required**

func indirectScribbleInteraction(any UIInteraction, shouldDelayFocusForElement: Self.ElementIdentifier) -> Bool

Allow the delegate to delay focusing an element.

**Required** Default implementation provided.

