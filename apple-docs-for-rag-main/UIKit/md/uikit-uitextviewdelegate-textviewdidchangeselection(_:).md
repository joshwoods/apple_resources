

- UIKit
- UITextViewDelegate
-  textViewDidChangeSelection(\_:) 

Instance Method

# textViewDidChangeSelection(\_:)

Tells the delegate when the text selection changes in the specified text view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textViewDidChangeSelection(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view whose selection changed.

## Discussion

Implementation of this method is optional. You can use the selectedRange property of the text view to get the new selection.

