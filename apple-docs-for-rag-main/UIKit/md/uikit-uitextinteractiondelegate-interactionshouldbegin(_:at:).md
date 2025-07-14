

- UIKit
- UITextInteractionDelegate
-  interactionShouldBegin(\_:at:) 

Instance Method

# interactionShouldBegin(\_:at:)

Asks the delegate whether the text interaction should begin.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func interactionShouldBegin(
    _ interaction: UITextInteraction,
    at point: CGPoint
) -> Bool
```

## Parameters 

`interaction`  

The text interaction that called this method.

`point`  

The position on the screen where the user is touching.

## Return Value

A Boolean value indicating whether the interaction should begin. Return true to let the interaction begin; otherwise, return false to prevent the interaction from beginning.

## See Also

### Handling text interaction events

func interactionWillBegin(UITextInteraction)

Tells the delegate that the text interaction will begin.

func interactionDidEnd(UITextInteraction)

Tells the delegate that the text interaction ended.

