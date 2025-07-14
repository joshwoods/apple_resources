

- Foundation
- UndoManager
-  canRedo 

Instance Property

# canRedo

A Boolean value that indicates whether the manager has any actions to redo.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var canRedo: Bool { get }
```

## Discussion

true if the manager has any actions to redo, otherwise false.

Because any undo operation registered clears the redo stack, this method posts an NSUndoManagerCheckpoint to allow clients to apply their pending operations before testing the redo stack.

## See Also

### Related Documentation

func redo()

Performs the operations in the last group on the redo stack, if there are any, recording them on the undo stack as a single group.

### Checking undo ability

var canUndo: Bool

A Boolean value that indicates whether the manager has any actions to undo.

