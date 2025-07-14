

- UIKit
- UITextPasteDelegate
-  textPasteConfigurationSupporting(\_:shouldAnimatePasteOf:to:) 

Instance Method

# textPasteConfigurationSupporting(\_:shouldAnimatePasteOf:to:)

Asks the delegate if the paste or drop operation should be animated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textPasteConfigurationSupporting(
    _ textPasteConfigurationSupporting: any UITextPasteConfigurationSupporting,
    shouldAnimatePasteOf attributedString: NSAttributedString,
    to textRange: UITextRange
) -> Bool
```

## Parameters 

`textPasteConfigurationSupporting`  

The object that received the paste or drop request.

`attributedString`  

The text that will be added to the text view.

`textRange`  

The position in the text view where the paste or drop operation will place the text.

## Return Value

false if the paste or drop operation should not be animated; otherwise, true.

## Discussion

If you don’t want the system to animate the paste or drop operation, implement this method and return false. The operation is animated if you return true or if this method isn’t implemented.

