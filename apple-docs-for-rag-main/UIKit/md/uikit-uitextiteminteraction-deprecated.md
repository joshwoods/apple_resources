

- UIKit
-  UITextItemInteraction Deprecated

Enumeration

# UITextItemInteraction

Constants that indicate the type of interaction the user expects to have with a URL or text attachment.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum UITextItemInteraction
```

## Topics

### Constants

case invokeDefaultAction

The user wants to perform the default action on the text item; for example, opening a URL.

case presentActions

The user wants to be presented with a list of actions that can be taken on the text item, such as opening the link in a different way or downloading content from the link.

case preview

The user wants to get a preview of the content represented by the text item, such as by initiating a peek and pop on a link.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the provided text attachment in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the specified URL in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the provided text attachment in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the specified URL in the specified range of text.

Deprecated

