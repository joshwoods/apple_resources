

- AppKit
- NSTextView
-  selectedRanges 

Instance Property

# selectedRanges

An array containing the ranges of characters selected in the receiver’s layout manager.

macOS

``` source
@MainActor
var selectedRanges: [NSValue] { get set }
```

## Discussion

The objects in the array are sorted, non-overlapping, non-contiguous, and (except for the case of a single range) have non-zero-length

## See Also

### Managing the selection

func setSelectedRange(NSRange)

Selects the specified range of characters in response to user action.

func setSelectedRange(NSRange, affinity: NSSelectionAffinity, stillSelecting: Bool)

Sets the selection to a range of characters in response to user action.

func setSelectedRanges([NSValue], affinity: NSSelectionAffinity, stillSelecting: Bool)

Sets the selection to the characters in an array of ranges in response to user action.

var selectionAffinity: NSSelectionAffinity

The preferred direction of selection.

var selectionGranularity: NSSelectionGranularity

The selection granularity for subsequent extension of a selection.

var insertionPointColor: NSColor!

The color of the insertion point.

func updateInsertionPointStateAndRestartTimer(Bool)

Updates the insertion point’s location and optionally restarts the blinking cursor timer.

var selectedTextAttributes: [NSAttributedString.Key : Any]

The attributes used to indicate the selection.

var markedTextAttributes: [NSAttributedString.Key : Any]?

The attributes used to draw marked text.

var linkTextAttributes: [NSAttributedString.Key : Any]?

The attributes used to draw the onscreen presentation of link text.

func characterIndexForInsertion(at: NSPoint) -> Int

Returns a character index appropriate for placing a zero-length selection for an insertion point associated with the mouse at the given point.

func updateCandidates()

