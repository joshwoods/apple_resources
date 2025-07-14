

- AppKit
- NSTextViewDelegate
-  textView(\_:shouldChangeTextInRanges:replacementStrings:) 

Instance Method

# textView(\_:shouldChangeTextInRanges:replacementStrings:)

Sent when a text view needs to determine if text in an array of specified ranges should be changed.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    shouldChangeTextInRanges affectedRanges: [NSValue],
    replacementStrings: [String]?
) -> Bool
```

## Parameters 

`textView`  

The text view sending the message. This is the first text view in a series shared by a layout manager, not necessarily the text view displaying the selected text.

`affectedRanges`  

The array of ranges of characters to be replaced. This array must be a non-nil, non-empty array of objects responding to the NSValue `rangeValue` method, and in addition its elements must be sorted, non-overlapping, non-contiguous, and (except for the case of a single range) have non-zero-length.

`replacementStrings`  

The array of strings that will replace the characters in `affectedRanges`, one string for each range; `nil` if only text attributes are being changed.

## Return Value

true to allow the replacement, or false to reject the change.

## See Also

### Setting Text Attributes

func textView(NSTextView, shouldChangeTextIn: NSRange, replacementString: String?) -> Bool

Sent when a text view needs to determine if text in a specified range should be changed.

func textView(NSTextView, shouldChangeTypingAttributes: [String : Any], toAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]

Sent when the typing attributes are changed.

func textViewDidChangeTypingAttributes(Notification)

Sent when a text view’s typing attributes change.

