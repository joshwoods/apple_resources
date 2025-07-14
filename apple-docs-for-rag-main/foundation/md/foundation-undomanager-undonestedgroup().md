

- Foundation
- UndoManager
-  undoNestedGroup() 

Instance Method

# undoNestedGroup()

Performs the undo operations in the last undo group (whether top-level or nested), recording the operations on the redo stack as a single group.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func undoNestedGroup()
```

## Discussion

Raises an `NSInternalInconsistencyException` if any undo operations have been registered since the last enableUndoRegistration() message.

This method posts an NSUndoManagerCheckpoint and NSUndoManagerWillUndoChange before it performs the undo operation, and it posts an NSUndoManagerDidUndoChange after it performs the undo operation.

## See Also

### Performing undo and redo

func undo()

Closes the top-level undo group if necessary, and then performs undo operations on the group.

func redo()

Performs the operations in the last group on the redo stack, if there are any, recording them on the undo stack as a single group.

