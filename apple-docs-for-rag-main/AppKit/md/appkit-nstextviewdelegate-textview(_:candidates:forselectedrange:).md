

- AppKit
- NSTextViewDelegate
-  textView(\_:candidates:forSelectedRange:) 

Instance Method

# textView(\_:candidates:forSelectedRange:)

Returns an array of text objects to include in a text selection.

macOS 10.12.2+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    candidates: [NSTextCheckingResult],
    forSelectedRange selectedRange: NSRange
) -> [NSTextCheckingResult]
```

## Return Value

An array of NSTextCheckingResult objects.

## See Also

### Managing the Selection

func textView(NSTextView, willChangeSelectionFromCharacterRange: NSRange, toCharacterRange: NSRange) -> NSRange

Returns the actual range to select.

func textView(NSTextView, willChangeSelectionFromCharacterRanges: [NSValue], toCharacterRanges: [NSValue]) -> [NSValue]

Returns the actual character ranges to select.

func textViewDidChangeSelection(Notification)

Sent when the selection changes in the text view.

func textView(NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

Returns an array of objects that represent the elements of a selection.

func textView(NSTextView, shouldSelectCandidateAt: Int) -> Bool

Returns a Boolean value that indicates whether to select the text object at the index.

func textView(NSTextView, shouldUpdateTouchBarItemIdentifiers: [NSTouchBarItem.Identifier]) -> [NSTouchBarItem.Identifier]

Returns and array of touch bar elements for the framework to update.

