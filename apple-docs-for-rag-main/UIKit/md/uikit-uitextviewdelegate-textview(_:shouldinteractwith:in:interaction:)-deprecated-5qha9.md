

- UIKit
- UITextViewDelegate
-  textView(\_:shouldInteractWith:in:interaction:) Deprecated

Instance Method

# textView(\_:shouldInteractWith:in:interaction:)

Asks the delegate whether the specified text view allows the specified type of user interaction with the provided text attachment in the specified range of text.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    shouldInteractWith textAttachment: NSTextAttachment,
    in characterRange: NSRange,
    interaction: UITextItemInteraction
) -> Bool
```

## Parameters 

`textView`  

The text view containing the text attachment.

`textAttachment`  

The text attachment.

`characterRange`  

The character range containing the text attachment.

`interaction`  

The type of interaction that is occurring (for possible values, see UITextItemInteraction).

## Return Value

true if interaction with the text attachment should be allowed; false if interaction should not be allowed.

## Discussion

A text view calls this method if the user taps or long-presses the text attachment and its image property is not `nil`. You can use this method to trigger an action in addition to displaying the text attachment inline with the text.

## See Also

### Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the specified URL in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the provided text attachment in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the specified URL in the specified range of text.

Deprecated

enum UITextItemInteraction

Constants that indicate the type of interaction the user expects to have with a URL or text attachment.

Deprecated

