

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:requestElementsIn:completion:) 

Instance Method

# indirectScribbleInteraction(\_:requestElementsIn:completion:)

Asks the delegate to return the locations of text input elements inside the specified rectangle of the view.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    requestElementsIn rect: CGRect,
    completion: @escaping ([Self.ElementIdentifier]) -> Void
)
```

**Required**

## Parameters 

`interaction`  

The interaction where the user finished writing.

`rect`  

The rect around the area where the user is trying to write, in the interaction’s view coordinate system. Return only the elements intersecting this rect.

`completion`  

A completion handler that you must call, either synchronously or asynchronously. Pass an array of identifiers of the available elements, or an empty array if there are no elements.

## Discussion

Each rectangle returned by the completion handler represents an area where the user can start writing even if it’s not a text input field itself.

## See Also

### Finding Elements and Frames

func indirectScribbleInteraction(any UIInteraction, frameForElement: Self.ElementIdentifier) -> CGRect

Asks the delegate to provide the frame of an element.

**Required**

