

- Foundation
- UndoManager
-  levelsOfUndo 

Instance Property

# levelsOfUndo

The maximum number of top-level undo groups the undo manager holds.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var levelsOfUndo: Int { get set }
```

## Discussion

An integer specifying the number of undo groups. A limit of `0` indicates no limit, so the manager never drops old undo groups.

When ending an undo group results in the number of groups exceeding this limit, the manager drops the oldest groups from the stack. The default is `0`.

If you change the limit to a level below the prior limit, the manager immediately drops old undo groups.

## See Also

### Related Documentation

func enableUndoRegistration()

Enables the recording of undo operations.

### Managing undo and redo stack depth

var undoCount: Int

The number of times you can invoke undo before there are no actions left to undo.

var redoCount: Int

The number of times you can invoke redo before there are no actions left to redo.

