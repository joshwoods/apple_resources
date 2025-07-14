

- UIKit
- UITextViewDelegate
-  textViewDidChange(\_:) 

Instance Method

# textViewDidChange(\_:)

Tells the delegate when the user changes the text or attributes in the specified text view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textViewDidChange(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view containing the changes.

## Discussion

The text view calls this method in response to user-initiated changes to the text. This method is not called in response to programmatically initiated changes.

Implementation of this method is optional.

## See Also

### Responding to text changes

func textView(UITextView, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Asks the delegate whether to replace the specified text in the text view.

