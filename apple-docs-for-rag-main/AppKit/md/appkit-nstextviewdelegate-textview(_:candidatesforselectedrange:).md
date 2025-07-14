

- AppKit
- NSTextViewDelegate
-  textView(\_:candidatesForSelectedRange:) 

Instance Method

# textView(\_:candidatesForSelectedRange:)

Returns an array of objects that represent the elements of a selection.

macOS 10.12.2+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    candidatesForSelectedRange selectedRange: NSRange
) -> [Any]?
```

## Return Value

An array of objects that represent the selection.

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

func textView(NSTextView, shouldSelectCandidateAt: Int) -> Bool

Returns a Boolean value that indicates whether to select the text object at the index.

func textView(NSTextView, shouldUpdateTouchBarItemIdentifiers: [NSTouchBarItem.Identifier]) -> [NSTouchBarItem.Identifier]

Returns and array of touch bar elements for the framework to update.

