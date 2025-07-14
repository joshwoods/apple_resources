

- AppKit
- NSTextView
-  isCoalescingUndo 

Instance Property

# isCoalescingUndo

A Boolean value that indicates whether undo coalescing is in progress.

macOS 10.6+

``` source
@MainActor
var isCoalescingUndo: Bool { get }
```

## Discussion

true if undo coalescing is in progress, otherwise false.

## See Also

### Supporting undo

func breakUndoCoalescing()

Informs the receiver that it should begin coalescing successive typing operations in a new undo grouping.

