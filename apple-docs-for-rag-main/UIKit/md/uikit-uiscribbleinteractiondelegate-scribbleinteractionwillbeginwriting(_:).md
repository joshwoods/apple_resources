

- UIKit
- UIScribbleInteractionDelegate
-  scribbleInteractionWillBeginWriting(\_:) 

Instance Method

# scribbleInteractionWillBeginWriting(\_:)

Informs the delegate when the user begins writing in the view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@MainActor
optional func scribbleInteractionWillBeginWriting(_ interaction: UIScribbleInteraction)
```

## Parameters 

`interaction`  

The interaction where the user started writing.

## Discussion

Use this method to hide custom placeholders or other UI elements that can interfere with writing.

## See Also

### Tracking Scribble input

func scribbleInteractionDidFinishWriting(UIScribbleInteraction)

Informs the delegate that the user stops writing in the view, after Scribble transcribes and enters the last word.

