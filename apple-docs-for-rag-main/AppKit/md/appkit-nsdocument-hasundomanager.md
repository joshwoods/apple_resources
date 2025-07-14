

- AppKit
- NSDocument
-  hasUndoManager 

Instance Property

# hasUndoManager

A Boolean value that indicates whether the document owns an undo manager object.

macOS

``` source
@MainActor
var hasUndoManager: Bool { get set }
```

## Discussion

If you change the value of this property to NO and the document already owns an UndoManager object, the document removes the undo manager as an observer of undo-related notifications and then removes its reference to the object.

## See Also

### Managing Undo and Redo Actions

var undoManager: UndoManager?

The object that the document uses to support undo/redo operations.

