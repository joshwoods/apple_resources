

- UIKit
- UITextViewDelegate
-  textViewShouldBeginEditing(\_:) 

Instance Method

# textViewShouldBeginEditing(\_:)

Asks the delegate whether to begin editing in the specified text view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textViewShouldBeginEditing(_ textView: UITextView) -> Bool
```

## Parameters 

`textView`  

The text view for which editing is about to begin.

## Return Value

true if an editing session should be initiated; otherwise, false to disallow editing.

## Discussion

When the user performs an action that would normally initiate an editing session, the text view calls this method first to see if editing should actually proceed. In most circumstances, you would simply return true from this method to allow editing to proceed.

Implementation of this method by the delegate is optional. If it is not present, editing proceeds as if this method had returned true.

## See Also

### Responding to editing notifications

func textViewDidBeginEditing(UITextView)

Tells the delegate when editing of the specified text view begins.

func textViewShouldEndEditing(UITextView) -> Bool

Asks the delegate whether to stop editing in the specified text view.

func textViewDidEndEditing(UITextView)

Tells the delegate when editing of the specified text view ends.

