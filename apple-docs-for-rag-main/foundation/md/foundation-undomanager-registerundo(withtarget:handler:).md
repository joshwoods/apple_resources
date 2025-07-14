

- Foundation
- UndoManager
-  registerUndo(withTarget:handler:) 

Instance Method

# registerUndo(withTarget:handler:)

Registers the specified closure to implement a single undo operation that the target receives.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
func registerUndo(
    withTarget target: TargetType,
    handler: @escaping (TargetType) -> Void
) where TargetType : AnyObject
```

## Parameters 

`target`  

The target of the undo operation.

The undo manager maintains an unowned reference to the `target` to prevent retain cycles.

`handler`  

A closure to execute when an operation is undone.

The closure takes a single argument, the target of the undo operation.

## Discussion

Use registerUndo(withTarget:handler:) to register a closure as an undo operation on the undo stack. The registered closure is then executed when `undo` is called and the undo operation occurs. The target needs to be a reference type so that its state can be undone or redone by the undo manager.

The following example demonstrates how you can use this method to register an undo operation that adds an element back into a mutable array.

```
var manager = UndoManager()
var bouquetSelection: NSMutableArray = ["lilac", "lavender"]
func pull(flower: String) {
    bouquetSelection.remove(flower)
    manager.registerUndo(withTarget: bouquetSelection) { $0.add(flower) }
}
pull(flower: "lilac")
// bouquetSelection == ["lavender"]
manager.undo()
// bouquetSelection == ["lavender", "lilac"]
```

To avoid retain cycles with the target, operate on the closure parameter rather than on variables in an outer scope that reference the same target. For example, in the code listing above, the closure operates on the `$0` parameter rather than directly on `bouquetSelection`.

## See Also

### Related Documentation

Introduction to Undo Architecture

### Registering undo operations

func registerUndo(withTarget: Any, selector: Selector, object: Any?)

Registers the selector of the specified target to implement a single undo operation that the target receives.

func prepare(withInvocationTarget: Any) -> Any

Prepares the undo manager for invocation-based undo with the given target as the subject of the next undo operation.

