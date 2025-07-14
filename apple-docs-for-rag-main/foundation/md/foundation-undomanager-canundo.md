

- Foundation
- UndoManager
-  canUndo 

Instance Property

# canUndo

A Boolean value that indicates whether the manager has any actions to undo.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var canUndo: Bool { get }
```

## Discussion

true if the manager has any actions to undo, otherwise false.

The return value doesn’t mean you can safely invoke undo() or undoNestedGroup()—you may have to close open undo groups first.

## See Also

### Related Documentation

func registerUndo(withTarget: Any, selector: Selector, object: Any?)

Registers the selector of the specified target to implement a single undo operation that the target receives.

func enableUndoRegistration()

Enables the recording of undo operations.

### Checking undo ability

var canRedo: Bool

A Boolean value that indicates whether the manager has any actions to redo.

