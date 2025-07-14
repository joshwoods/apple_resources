

- AppKit
- NSTextView
-  linkTextAttributes 

Instance Property

# linkTextAttributes

The attributes used to draw the onscreen presentation of link text.

macOS

``` source
@MainActor
var linkTextAttributes: [NSAttributedString.Key : Any]? { get set }
```

## Discussion

Link text attributes are applied as temporary attributes to any text with a link attribute. Candidates include those attributes that do not affect layout.

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

func characterIndexForInsertion(at: NSPoint) -> Int

Returns a character index appropriate for placing a zero-length selection for an insertion point associated with the mouse at the given point.

func updateCandidates()

