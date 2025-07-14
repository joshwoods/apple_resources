

- Foundation
- UndoManager
-  redo() 

Instance Method

# redo()

Performs the operations in the last group on the redo stack, if there are any, recording them on the undo stack as a single group.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func redo()
```

## Discussion

Raises an internalInconsistencyException if the method is invoked during an undo operation.

This method posts an NSUndoManagerCheckpoint and NSUndoManagerWillRedoChange before it performs the redo operation, and it posts the NSUndoManagerDidRedoChange after it performs the redo operation.

## See Also

### Related Documentation

func registerUndo(withTarget: Any, selector: Selector, object: Any?)

Registers the selector of the specified target to implement a single undo operation that the target receives.

### Performing undo and redo

func undo()

Closes the top-level undo group if necessary, and then performs undo operations on the group.

func undoNestedGroup()

Performs the undo operations in the last undo group (whether top-level or nested), recording the operations on the redo stack as a single group.

