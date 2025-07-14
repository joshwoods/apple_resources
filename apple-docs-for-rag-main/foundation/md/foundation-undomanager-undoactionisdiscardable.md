

- Foundation
- UndoManager
-  undoActionIsDiscardable 

Instance Property

# undoActionIsDiscardable

A Boolean value that indicates whether the next undo action is discardable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var undoActionIsDiscardable: Bool { get }
```

## Discussion

true if the action is discardable; false otherwise.

Specifies that the latest undo action may be safely discarded when a document can not be saved for any reason. These are typically actions that don’t affect persistent state.

An example might be an undo action that changes the viewable area of a document.

## See Also

### Using discardable undo and redo actions

func setActionIsDiscardable(Bool)

Sets whether the next undo or redo action is discardable.

var redoActionIsDiscardable: Bool

A Boolean value that indicates whether the next redo action is discardable.

