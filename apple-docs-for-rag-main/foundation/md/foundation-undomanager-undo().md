

- Foundation
- UndoManager
-  undo() 

Instance Method

# undo()

Closes the top-level undo group if necessary, and then performs undo operations on the group.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func undo()
```

## Discussion

After closing the top-level undo group, this method invokes undoNestedGroup().

This method also invokes endUndoGrouping() if the nesting level is 1. Raises an `NSInternalInconsistencyException` if more than one undo group is open (that is, if the last group isn’t at the top level).

This method posts an NSUndoManagerCheckpoint.

## See Also

### Related Documentation

var groupingLevel: Int

The number of nested undo groups (or redo groups, if redo is the most recent operation) in the current event loop.

func enableUndoRegistration()

Enables the recording of undo operations.

### Performing undo and redo

func undoNestedGroup()

Performs the undo operations in the last undo group (whether top-level or nested), recording the operations on the redo stack as a single group.

func redo()

Performs the operations in the last group on the redo stack, if there are any, recording them on the undo stack as a single group.

