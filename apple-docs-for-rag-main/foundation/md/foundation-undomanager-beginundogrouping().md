

- Foundation
- UndoManager
-  beginUndoGrouping() 

Instance Method

# beginUndoGrouping()

Marks the beginning of an undo group.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func beginUndoGrouping()
```

## Discussion

All individual undo operations before a subsequent endUndoGrouping() message are grouped together and reversed by a later undo() message. By default undo groups are begun automatically at the start of the event loop, but you can begin your own undo groups with this method, and nest them within other groups.

This method posts an NSUndoManagerCheckpoint unless a top-level undo is in progress. It posts an NSUndoManagerDidOpenUndoGroup if a new group was successfully created.

## See Also

### Creating undo groups

func endUndoGrouping()

Marks the end of an undo group.

var groupsByEvent: Bool

A Boolean value that indicates whether the manager automatically creates undo groups around each pass of the run loop.

var groupingLevel: Int

The number of nested undo groups (or redo groups, if redo is the most recent operation) in the current event loop.

