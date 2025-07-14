

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:didFinishWritingInElement:) 

Instance Method

# indirectScribbleInteraction(\_:didFinishWritingInElement:)

Informs the delegate when the user finishes writing.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    didFinishWritingInElement elementIdentifier: Self.ElementIdentifier
)
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction where the user finished writing.

`elementIdentifier`  

The identifier of the element that should receive focus.

## Discussion

Use this to reset placeholders or other UI elements, if appropriate, to their state from before the user started writing.

## Default Implementations

### UIIndirectScribbleInteractionDelegate Implementations

func indirectScribbleInteraction(any UIInteraction, didFinishWritingInElement: Self.ElementIdentifier)

## See Also

### Tracking Scribble Input

func indirectScribbleInteraction(any UIInteraction, willBeginWritingInElement: Self.ElementIdentifier)

Informs the delegate when the user begins writing.

**Required** Default implementation provided.

