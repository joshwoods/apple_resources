

- Foundation
-  NSUndoCloseGroupingRunLoopOrdering 

Global Variable

# NSUndoCloseGroupingRunLoopOrdering

A priority to use when using a run loop to close an undo group.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSUndoCloseGroupingRunLoopOrdering: Int
```

## Discussion

Use this value as the `order` parameter if you call perform(_:target:argument:order:modes:) to have a RunLoop perform a selector that closes an undo group.

## See Also

### Working with run loops

var runLoopModes: [RunLoop.Mode]

The modes governing the types of input to handle during a cycle of the run loop.

