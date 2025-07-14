

- UIKit
- UIScribbleInteractionDelegate
-  scribbleInteractionDidFinishWriting(\_:) 

Instance Method

# scribbleInteractionDidFinishWriting(\_:)

Informs the delegate that the user stops writing in the view, after Scribble transcribes and enters the last word.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@MainActor
optional func scribbleInteractionDidFinishWriting(_ interaction: UIScribbleInteraction)
```

## Parameters 

`interaction`  

The interaction where the user finished writing.

## Discussion

Use this to reset placeholders or other UI elements, if appropriate, to their state from before the user started writing.

## See Also

### Tracking Scribble input

func scribbleInteractionWillBeginWriting(UIScribbleInteraction)

Informs the delegate when the user begins writing in the view.

