

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:frameForElement:) 

Instance Method

# indirectScribbleInteraction(\_:frameForElement:)

Asks the delegate to provide the frame of an element.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    frameForElement elementIdentifier: Self.ElementIdentifier
) -> CGRect
```

**Required**

## Parameters 

`interaction`  

The interaction requesting to focus an element.

`elementIdentifier`  

The identifier of the element that should receive focus.

## Return Value

Returns the frame for the element, in the view coordinate system of the interaction.

## See Also

### Finding Elements and Frames

func indirectScribbleInteraction(any UIInteraction, requestElementsIn: CGRect, completion: ([Self.ElementIdentifier]) -> Void)

Asks the delegate to return the locations of text input elements inside the specified rectangle of the view.

**Required**

