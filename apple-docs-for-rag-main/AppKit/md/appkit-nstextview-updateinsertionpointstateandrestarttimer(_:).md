

- AppKit
- NSTextView
-  updateInsertionPointStateAndRestartTimer(\_:) 

Instance Method

# updateInsertionPointStateAndRestartTimer(\_:)

Updates the insertion point’s location and optionally restarts the blinking cursor timer.

macOS

``` source
@MainActor
func updateInsertionPointStateAndRestartTimer(_ restartFlag: Bool)
```

## Parameters 

`restartFlag`  

true to restart the blinking cursor timer, false otherwise.

## Discussion

This method is invoked automatically whenever the insertion point needs to be moved; you should never need to invoke it directly, but you can override it to modify insertion point behavior.

## See Also

### Related Documentation

var shouldDrawInsertionPoint: Bool

A Boolean value that determines whether the receiver should draw its insertion point.

func drawInsertionPoint(in: NSRect, color: NSColor, turnedOn: Bool)

Draws or erases the insertion point.

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

var selectedTextAttributes: [NSAttributedString.Key : Any]

The attributes used to indicate the selection.

var markedTextAttributes: [NSAttributedString.Key : Any]?

The attributes used to draw marked text.

var linkTextAttributes: [NSAttributedString.Key : Any]?

The attributes used to draw the onscreen presentation of link text.

func characterIndexForInsertion(at: NSPoint) -> Int

Returns a character index appropriate for placing a zero-length selection for an insertion point associated with the mouse at the given point.

func updateCandidates()

