

- AppKit
- NSTextViewDelegate
-  textView(\_:shouldChangeTextIn:replacementString:) 

Instance Method

# textView(\_:shouldChangeTextIn:replacementString:)

Sent when a text view needs to determine if text in a specified range should be changed.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    shouldChangeTextIn affectedCharRange: NSRange,
    replacementString: String?
) -> Bool
```

## Parameters 

`textView`  

The text view sending the message. This is the first text view in a series shared by a layout manager, not necessarily the text view displaying the selected text.

`affectedCharRange`  

The range of characters to be replaced.

`replacementString`  

The characters that will replace the characters in `affectedCharRange`; `nil` if only text attributes are being changed.

## Return Value

true to allow the replacement, or false to reject the change.

## Discussion

If a delegate implements this method and not its multiple-selection replacement, textView(_:shouldChangeTextInRanges:replacementStrings:), it is called with an appropriate range and string. If a delegate implements the new method, then this one is ignored.

## See Also

### Setting Text Attributes

func textView(NSTextView, shouldChangeTextInRanges: [NSValue], replacementStrings: [String]?) -> Bool

Sent when a text view needs to determine if text in an array of specified ranges should be changed.

func textView(NSTextView, shouldChangeTypingAttributes: [String : Any], toAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]

Sent when the typing attributes are changed.

func textViewDidChangeTypingAttributes(Notification)

Sent when a text view’s typing attributes change.

