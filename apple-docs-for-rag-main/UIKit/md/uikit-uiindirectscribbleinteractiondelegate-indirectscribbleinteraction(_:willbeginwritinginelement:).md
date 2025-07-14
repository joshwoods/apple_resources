

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:willBeginWritingInElement:) 

Instance Method

# indirectScribbleInteraction(\_:willBeginWritingInElement:)

Informs the delegate when the user begins writing.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    willBeginWritingInElement elementIdentifier: Self.ElementIdentifier
)
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction where the user started writing.

`elementIdentifier`  

The identifier of the element that should receive focus.

## Discussion

Use this to hide custom placeholders or other UI elements that can interfere with writing.

## Default Implementations

### UIIndirectScribbleInteractionDelegate Implementations

func indirectScribbleInteraction(any UIInteraction, willBeginWritingInElement: Self.ElementIdentifier)

## See Also

### Tracking Scribble Input

func indirectScribbleInteraction(any UIInteraction, didFinishWritingInElement: Self.ElementIdentifier)

Informs the delegate when the user finishes writing.

**Required** Default implementation provided.

