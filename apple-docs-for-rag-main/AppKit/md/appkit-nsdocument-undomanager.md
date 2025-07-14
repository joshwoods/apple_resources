

- AppKit
- NSDocument
-  undoManager 

Instance Property

# undoManager

The object that the document uses to support undo/redo operations.

macOS

``` source
@MainActor
var undoManager: UndoManager? { get set }
```

## Discussion

When the hasUndoManager property is true, accessing this property creates an UndoManager before returning it. If the hasUndoManager property is false, the value of this property is `nil` by default. Assigning an undo manager to this property stores a reference to the object and automatically changes the hasUndoManager property to true.

Whether you assign an undo manager or let the document create one, the document registers itself as an observer of various UndoManager notifications so that appropriate document actions are stored on the undo stack.

## See Also

### Managing Undo and Redo Actions

var hasUndoManager: Bool

A Boolean value that indicates whether the document owns an undo manager object.

