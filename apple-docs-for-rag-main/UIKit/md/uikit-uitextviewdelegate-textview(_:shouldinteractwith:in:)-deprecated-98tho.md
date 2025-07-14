

- UIKit
- UITextViewDelegate
-  textView(\_:shouldInteractWith:in:) Deprecated

Instance Method

# textView(\_:shouldInteractWith:in:)

Asks the delegate whether the specified text view allows user interaction with the specified URL in the specified range of text.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    shouldInteractWith URL: URL,
    in characterRange: NSRange
) -> Bool
```

Deprecated

Use textView(_:shouldInteractWith:in:interaction:) instead.

## Parameters 

`textView`  

The text view containing the text attachment.

`URL`  

The URL to be processed.

`characterRange`  

The character range containing the URL.

## Return Value

true if interaction with the URL should be allowed; false if interaction should not be allowed.

## Discussion

The text view calls this method if the user taps or long-presses the URL link. Implementation of this method is optional. By default, the text view opens the application responsible for handling the URL type and passes it the URL. You can use this method to trigger an alternative action, such as displaying the web content at the URL in a web view within the current application.

Important

Links in text views are interactive only if the text view is selectable but noneditable. That is, if the value of the `UITextView` isSelectable property is true and the isEditable property is false.

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

enum UITextItemInteraction

Constants that indicate the type of interaction the user expects to have with a URL or text attachment.

Deprecated

