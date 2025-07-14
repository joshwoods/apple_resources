

- UIKit
- UITextViewDelegate
-  textViewDidEndEditing(\_:) 

Instance Method

# textViewDidEndEditing(\_:)

Tells the delegate when editing of the specified text view ends.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textViewDidEndEditing(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view in which editing ended.

## Discussion

Implementation of this method is optional. A text view sends this message to its delegate after it closes out any pending edits and resigns its first responder status. You can use this method to tear down any data structures or change any state information that you set when editing began.

## See Also

### Responding to editing notifications

func textViewShouldBeginEditing(UITextView) -> Bool

Asks the delegate whether to begin editing in the specified text view.

func textViewDidBeginEditing(UITextView)

Tells the delegate when editing of the specified text view begins.

func textViewShouldEndEditing(UITextView) -> Bool

Asks the delegate whether to stop editing in the specified text view.

