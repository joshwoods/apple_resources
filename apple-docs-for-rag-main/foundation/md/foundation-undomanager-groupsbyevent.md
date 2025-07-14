

- Foundation
- UndoManager
-  groupsByEvent 

Instance Property

# groupsByEvent

A Boolean value that indicates whether the manager automatically creates undo groups around each pass of the run loop.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var groupsByEvent: Bool { get set }
```

## Discussion

true if the manager automatically creates undo groups around each pass of the run loop, otherwise false.

The default is true. If you turn automatic grouping off, you must close groups explicitly before invoking either undo() or undoNestedGroup().

## See Also

### Creating undo groups

func beginUndoGrouping()

Marks the beginning of an undo group.

func endUndoGrouping()

Marks the end of an undo group.

var groupingLevel: Int

The number of nested undo groups (or redo groups, if redo is the most recent operation) in the current event loop.

