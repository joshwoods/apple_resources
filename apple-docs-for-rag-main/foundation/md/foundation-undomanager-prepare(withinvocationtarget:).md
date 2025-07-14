

- Foundation
- UndoManager
-  prepare(withInvocationTarget:) 

Instance Method

# prepare(withInvocationTarget:)

Prepares the undo manager for invocation-based undo with the given target as the subject of the next undo operation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func prepare(withInvocationTarget target: Any) -> Any
```

## Parameters 

`target`  

The target of the undo operation.

The undo manager maintains a weak reference to `target`.

## Return Value

A proxy object that forwards messages to the undo manager for recording as undo actions.

## See Also

### Registering undo operations

func registerUndo&lt;TargetType>(withTarget: TargetType, handler: (TargetType) -> Void)

Registers the specified closure to implement a single undo operation that the target receives.

func registerUndo(withTarget: Any, selector: Selector, object: Any?)

Registers the selector of the specified target to implement a single undo operation that the target receives.

