

- UIKit
- UITextViewDelegate
-  textView(\_:shouldInteractWith:in:interaction:) Deprecated

Instance Method

# textView(\_:shouldInteractWith:in:interaction:)

Asks the delegate whether the specified text view allows the specified type of user interaction with the specified URL in the specified range of text.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    shouldInteractWith URL: URL,
    in characterRange: NSRange,
    interaction: UITextItemInteraction
) -> Bool
```

## Parameters 

`textView`  

The text view containing the text attachment.

`URL`  

The URL to be processed.

`characterRange`  

The character range containing the URL.

`interaction`  

The type of interaction that is occurring (for possible values, see UITextItemInteraction).

## Return Value

true if interaction with the URL should be allowed; false if interaction should not be allowed.

## Discussion

This method is called on only the first interaction with the URL link. For example, this method is called when the user wants their first interaction with a URL to display a list of actions they can take; if the user chooses an open action from the list, this method is not called, because “open” represents the second interaction with the same URL.

Important

Links in text views are interactive only if the text view is selectable but noneditable. That is, if the value of the UITextView isSelectable property is true and the isEditable property is false.

## See Also

### Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the provided text attachment in the specified range of text.

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

