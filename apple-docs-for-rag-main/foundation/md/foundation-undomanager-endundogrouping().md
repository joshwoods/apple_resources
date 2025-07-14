

- Foundation
- UndoManager
-  endUndoGrouping() 

Instance Method

# endUndoGrouping()

Marks the end of an undo group.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func endUndoGrouping()
```

## Discussion

All individual undo operations back to the matching beginUndoGrouping() message are grouped together and reversed by a later undo() or undoNestedGroup() message. Undo groups can be nested, thus providing functionality similar to nested transactions. Raises an `NSInternalInconsistencyException` if there’s no beginUndoGrouping() message in effect.

This method posts an NSUndoManagerCheckpoint and an NSUndoManagerDidCloseUndoGroup just before the group is closed.

## See Also

### Related Documentation

var levelsOfUndo: Int

The maximum number of top-level undo groups the undo manager holds.

### Creating undo groups

func beginUndoGrouping()

Marks the beginning of an undo group.

var groupsByEvent: Bool

A Boolean value that indicates whether the manager automatically creates undo groups around each pass of the run loop.

var groupingLevel: Int

The number of nested undo groups (or redo groups, if redo is the most recent operation) in the current event loop.

