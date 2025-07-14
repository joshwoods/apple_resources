

- AppKit
- NSTextViewDelegate
-  textView(\_:shouldChangeTypingAttributes:toAttributes:) 

Instance Method

# textView(\_:shouldChangeTypingAttributes:toAttributes:)

Sent when the typing attributes are changed.

macOS 10.0+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    shouldChangeTypingAttributes oldTypingAttributes: [String : Any] = [:],
    toAttributes newTypingAttributes: [NSAttributedString.Key : Any] = [:]
) -> [NSAttributedString.Key : Any]
```

## Parameters 

`textView`  

The text view sending the message.

`oldTypingAttributes`  

The old typing attributes.

`newTypingAttributes`  

The proposed typing attributes.

## Return Value

The actual new typing attributes.

## See Also

### Setting Text Attributes

func textView(NSTextView, shouldChangeTextIn: NSRange, replacementString: String?) -> Bool

Sent when a text view needs to determine if text in a specified range should be changed.

func textView(NSTextView, shouldChangeTextInRanges: [NSValue], replacementStrings: [String]?) -> Bool

Sent when a text view needs to determine if text in an array of specified ranges should be changed.

func textViewDidChangeTypingAttributes(Notification)

Sent when a text view’s typing attributes change.

