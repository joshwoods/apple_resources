

- UIKit
- UITextInteractionDelegate
-  interactionDidEnd(\_:) 

Instance Method

# interactionDidEnd(\_:)

Tells the delegate that the text interaction ended.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func interactionDidEnd(_ interaction: UITextInteraction)
```

## Parameters 

`interaction`  

The text interaction that called this method.

## See Also

### Handling text interaction events

func interactionShouldBegin(UITextInteraction, at: CGPoint) -> Bool

Asks the delegate whether the text interaction should begin.

func interactionWillBegin(UITextInteraction)

Tells the delegate that the text interaction will begin.

