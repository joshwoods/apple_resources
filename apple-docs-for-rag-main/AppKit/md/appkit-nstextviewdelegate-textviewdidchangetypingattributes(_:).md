

- AppKit
- NSTextViewDelegate
-  textViewDidChangeTypingAttributes(\_:) 

Instance Method

# textViewDidChangeTypingAttributes(\_:)

Sent when a text view’s typing attributes change.

macOS 10.10+

``` source
@MainActor
optional func textViewDidChangeTypingAttributes(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didChangeTypingAttributesNotification.

## See Also

### Setting Text Attributes

func textView(NSTextView, shouldChangeTextIn: NSRange, replacementString: String?) -> Bool

Sent when a text view needs to determine if text in a specified range should be changed.

func textView(NSTextView, shouldChangeTextInRanges: [NSValue], replacementStrings: [String]?) -> Bool

Sent when a text view needs to determine if text in an array of specified ranges should be changed.

func textView(NSTextView, shouldChangeTypingAttributes: [String : Any], toAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]

Sent when the typing attributes are changed.

