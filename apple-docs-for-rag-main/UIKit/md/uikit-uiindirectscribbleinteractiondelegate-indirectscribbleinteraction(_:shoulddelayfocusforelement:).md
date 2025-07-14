

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:shouldDelayFocusForElement:) 

Instance Method

# indirectScribbleInteraction(\_:shouldDelayFocusForElement:)

Allow the delegate to delay focusing an element.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    shouldDelayFocusForElement elementIdentifier: Self.ElementIdentifier
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction asking about delaying focus.

`elementIdentifier`  

The identifier of the element the interaction is asking about.

## Return Value

Return true to delay focusing the element; the default is false.

## Default Implementations

### UIIndirectScribbleInteractionDelegate Implementations

func indirectScribbleInteraction(any UIInteraction, shouldDelayFocusForElement: Self.ElementIdentifier) -> Bool

## See Also

### Managing Focus

func indirectScribbleInteraction(any UIInteraction, isElementFocused: Self.ElementIdentifier) -> Bool

Asks the delegate if an element is currently focused, according to the internal state of the interaction’s view.

**Required**

func indirectScribbleInteraction(any UIInteraction, focusElementIfNeeded: Self.ElementIdentifier, referencePoint: CGPoint, completion: ((any UIResponder &amp; UITextInput)?) -> Void)

Asks the delegate to focus an element to handle text edits.

**Required**

