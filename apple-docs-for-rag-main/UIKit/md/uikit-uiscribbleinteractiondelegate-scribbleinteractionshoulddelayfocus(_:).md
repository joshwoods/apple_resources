

- UIKit
- UIScribbleInteractionDelegate
-  scribbleInteractionShouldDelayFocus(\_:) 

Instance Method

# scribbleInteractionShouldDelayFocus(\_:)

Tells the delegate to delay focusing the text input view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@MainActor
optional func scribbleInteractionShouldDelayFocus(_ interaction: UIScribbleInteraction) -> Bool
```

## Parameters 

`interaction`  

The text input view asking about delaying focus.

## Return Value

Return `true` to delay focusing the text input, `false` otherwise.

## Discussion

Normally, Scribble focuses the target input as soon as the user starts writing. If you return `true` from this callback, Scribble waits until the user pauses briefly while writing. This is useful in cases where the view shifts or transforms when becoming first responder, which can be disruptive to a user trying to write in the field.

It’s preferable to adjust the UI behavior and minimize these kinds transformations to avoid the layout changes. Only use this method as a last resort, since transcription happens all at once instead of incrementally.

## See Also

### Allowing and controlling Scribble interactions

func scribbleInteraction(UIScribbleInteraction, shouldBeginAt: CGPoint) -> Bool

Returns a Boolean value that indicates whether the delegate should allow writing at a specific location in the view.

