

- Foundation
- UndoManager
-  isRedoing 

Instance Property

# isRedoing

Returns a Boolean value that indicates whether the manager is in the process of performing a redo action.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isRedoing: Bool { get }
```

## Discussion

The value is true if the manager is performing its redo() method, otherwise false.

## See Also

### Checking whether undo or redo is in process

var isUndoing: Bool

Returns a Boolean value that indicates whether the manager is in the process of performing an undo action.

