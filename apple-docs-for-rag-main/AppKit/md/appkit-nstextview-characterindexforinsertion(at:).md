

- AppKit
- NSTextView
-  characterIndexForInsertion(at:) 

Instance Method

# characterIndexForInsertion(at:)

Returns a character index appropriate for placing a zero-length selection for an insertion point associated with the mouse at the given point.

macOS 10.5+

``` source
@MainActor
func characterIndexForInsertion(at point: NSPoint) -> Int
```

## Parameters 

`point`  

The point for which to return an index, in view coordinates.

## Return Value

The character index for the insertion point.

## Discussion

This method should be used for insertion points associated with mouse clicks, drag events, and so forth. For other purposes, it is better to use `NSLayoutManager` methods.

The `NSTextInput` method characterIndexForPoint: is not suitable for this role; it is intended only for uses related to text input methods.

## See Also

### Managing the selection

var selectedRanges: [NSValue]

An array containing the ranges of characters selected in the receiver’s layout manager.

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

func updateCandidates()

