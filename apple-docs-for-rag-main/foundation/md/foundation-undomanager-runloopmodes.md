

- Foundation
- UndoManager
-  runLoopModes 

Instance Property

# runLoopModes

The modes governing the types of input to handle during a cycle of the run loop.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var runLoopModes: [RunLoop.Mode] { get set }
```

## Discussion

An array of string constants specifying the current run-loop modes.

By default, the sole run-loop mode is `NSDefaultRunLoopMode` (which excludes data from `NSConnection` objects). Some examples of other uses are to limit the input to data received during a mouse-tracking session by setting the mode to `NSEventTrackingRunLoopMode`, or limit it to data received from a modal panel with `NSModalPanelRunLoopMode`.

## See Also

### Related Documentation

func perform(Selector, target: Any, argument: Any?, order: Int, modes: [RunLoop.Mode])

Schedules the sending of a message on the receiver.

### Working with run loops

let NSUndoCloseGroupingRunLoopOrdering: Int

A priority to use when using a run loop to close an undo group.

