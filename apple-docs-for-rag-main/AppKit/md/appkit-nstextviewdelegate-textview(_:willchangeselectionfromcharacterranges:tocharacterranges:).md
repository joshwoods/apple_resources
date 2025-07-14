

- AppKit
- NSTextViewDelegate
-  textView(\_:willChangeSelectionFromCharacterRanges:toCharacterRanges:) 

Instance Method

# textView(\_:willChangeSelectionFromCharacterRanges:toCharacterRanges:)

Returns the actual character ranges to select.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    willChangeSelectionFromCharacterRanges oldSelectedCharRanges: [NSValue],
    toCharacterRanges newSelectedCharRanges: [NSValue]
) -> [NSValue]
```

## Parameters 

`textView`  

The text view sending the message. This is the first text view in a series shared by a layout manager, not necessarily the text view displaying the selected text.

`oldSelectedCharRanges`  

An array containing the original ranges of the selection. This must be a non-`nil`, non-empty array of objects responding to the `NSValue` method `rangeValue`, and in addition its elements must be sorted, non-overlapping, non-contiguous, and (except for the case of a single range) have non-zero-length.

`newSelectedCharRanges`  

An array containing the proposed character ranges for the new selection. This must be a non-`nil`, non-empty array of objects responding to the `NSValue` method `rangeValue`, and in addition its elements must be sorted, non-overlapping, non-contiguous, and (except for the case of a single range) have non-zero-length.

## Return Value

An array containing the actual character ranges for the new selection.

## Discussion

Invoked before an `NSTextView` object finishes changing the selection—that is, when the last argument to a setSelectedRange(_:affinity:stillSelecting:) or setSelectedRanges(_:affinity:stillSelecting:) message is false.

Non-selectable text views do not process any mouse events. If for some reason it is necessary to disallow user selection change in a text view that handles mouse events, this can be achieved by making the text view selectable but implementing this delegate method to disallow selection changes.

If a delegate implements both this method and textView(_:willChangeSelectionFromCharacterRange:toCharacterRange:), then the latter is ignored.

## See Also

### Managing the Selection

func textView(NSTextView, willChangeSelectionFromCharacterRange: NSRange, toCharacterRange: NSRange) -> NSRange

Returns the actual range to select.

func textViewDidChangeSelection(Notification)

Sent when the selection changes in the text view.

func textView(NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

Returns an array of text objects to include in a text selection.

func textView(NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

Returns an array of objects that represent the elements of a selection.

func textView(NSTextView, shouldSelectCandidateAt: Int) -> Bool

Returns a Boolean value that indicates whether to select the text object at the index.

func textView(NSTextView, shouldUpdateTouchBarItemIdentifiers: [NSTouchBarItem.Identifier]) -> [NSTouchBarItem.Identifier]

Returns and array of touch bar elements for the framework to update.

