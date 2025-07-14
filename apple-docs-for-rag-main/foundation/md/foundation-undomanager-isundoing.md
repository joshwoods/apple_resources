

- Foundation
- UndoManager
-  isUndoing 

Instance Property

# isUndoing

Returns a Boolean value that indicates whether the manager is in the process of performing an undo action.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isUndoing: Bool { get }
```

## Discussion

The value is true if the manager is performing its undo() or undoNestedGroup() method, otherwise false.

## See Also

### Checking whether undo or redo is in process

var isRedoing: Bool

Returns a Boolean value that indicates whether the manager is in the process of performing a redo action.

