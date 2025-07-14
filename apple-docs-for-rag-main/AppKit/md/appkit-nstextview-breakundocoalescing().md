

- AppKit
- NSTextView
-  breakUndoCoalescing() 

Instance Method

# breakUndoCoalescing()

Informs the receiver that it should begin coalescing successive typing operations in a new undo grouping.

macOS

``` source
@MainActor
func breakUndoCoalescing()
```

## Discussion

This method should be invoked when saving the receiver’s contents to preserve proper tracking of unsaved changes and the document’s dirty state.

## See Also

### Supporting undo

var isCoalescingUndo: Bool

A Boolean value that indicates whether undo coalescing is in progress.

