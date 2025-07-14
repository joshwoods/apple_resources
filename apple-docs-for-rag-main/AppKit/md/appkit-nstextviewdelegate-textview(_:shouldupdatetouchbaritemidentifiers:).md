

- AppKit
- NSTextViewDelegate
-  textView(\_:shouldUpdateTouchBarItemIdentifiers:) 

Instance Method

# textView(\_:shouldUpdateTouchBarItemIdentifiers:)

Returns and array of touch bar elements for the framework to update.

macOS 10.12.2+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    shouldUpdateTouchBarItemIdentifiers identifiers: [NSTouchBarItem.Identifier]
) -> [NSTouchBarItem.Identifier]
```

## Parameters 

`textView`  

The text view that sent the message.

`identifiers`  

An array of touch bar identifiers to evaluate.

## Return Value

Returns an array of NSTouchBarItem.Identifier elements for framework to update.

## See Also

### Managing the Selection

func textView(NSTextView, willChangeSelectionFromCharacterRange: NSRange, toCharacterRange: NSRange) -> NSRange

Returns the actual range to select.

func textView(NSTextView, willChangeSelectionFromCharacterRanges: [NSValue], toCharacterRanges: [NSValue]) -> [NSValue]

Returns the actual character ranges to select.

func textViewDidChangeSelection(Notification)

Sent when the selection changes in the text view.

func textView(NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

Returns an array of text objects to include in a text selection.

func textView(NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

Returns an array of objects that represent the elements of a selection.

func textView(NSTextView, shouldSelectCandidateAt: Int) -> Bool

Returns a Boolean value that indicates whether to select the text object at the index.

