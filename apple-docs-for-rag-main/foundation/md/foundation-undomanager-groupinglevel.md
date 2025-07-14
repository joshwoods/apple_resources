

- Foundation
- UndoManager
-  groupingLevel 

Instance Property

# groupingLevel

The number of nested undo groups (or redo groups, if redo is the most recent operation) in the current event loop.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var groupingLevel: Int { get }
```

## Discussion

An integer indicating the number of nested groups. If 0 is returned, there is no open undo or redo group.

## See Also

### Related Documentation

var levelsOfUndo: Int

The maximum number of top-level undo groups the undo manager holds.

### Creating undo groups

func beginUndoGrouping()

Marks the beginning of an undo group.

func endUndoGrouping()

Marks the end of an undo group.

var groupsByEvent: Bool

A Boolean value that indicates whether the manager automatically creates undo groups around each pass of the run loop.

