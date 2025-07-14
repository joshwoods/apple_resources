

- Foundation
- UndoManager
-  undoCount 

Instance Property

# undoCount

The number of times you can invoke undo before there are no actions left to undo.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
var undoCount: Int { get }
```

## Discussion

A nonzero value doesn’t imply you can safely invoke undo() immediately, because you may have to close open undo groups first.

## See Also

### Managing undo and redo stack depth

var levelsOfUndo: Int

The maximum number of top-level undo groups the undo manager holds.

var redoCount: Int

The number of times you can invoke redo before there are no actions left to redo.

