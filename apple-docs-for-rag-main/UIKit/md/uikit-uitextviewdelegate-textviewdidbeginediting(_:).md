

- UIKit
- UITextViewDelegate
-  textViewDidBeginEditing(\_:) 

Instance Method

# textViewDidBeginEditing(\_:)

Tells the delegate when editing of the specified text view begins.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textViewDidBeginEditing(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view in which editing began.

## Discussion

Implementation of this method is optional. A text view sends this message to its delegate immediately after the user initiates editing in a text view and before any changes are actually made. You can use this method to set up any editing-related data structures and generally prepare your delegate to receive future editing messages.

## See Also

### Responding to editing notifications

func textViewShouldBeginEditing(UITextView) -> Bool

Asks the delegate whether to begin editing in the specified text view.

func textViewShouldEndEditing(UITextView) -> Bool

Asks the delegate whether to stop editing in the specified text view.

func textViewDidEndEditing(UITextView)

Tells the delegate when editing of the specified text view ends.

