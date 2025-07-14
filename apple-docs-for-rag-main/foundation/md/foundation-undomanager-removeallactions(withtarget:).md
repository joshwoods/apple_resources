

- Foundation
- UndoManager
-  removeAllActions(withTarget:) 

Instance Method

# removeAllActions(withTarget:)

Clears the undo and redo stacks of all operations involving the specified target as the recipient of the undo message.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeAllActions(withTarget target: Any)
```

## Parameters 

`target`  

The recipient of the undo messages to be removed.

## Discussion

Doesn’t re-enable the manager if it’s disabled.

## See Also

### Related Documentation

func enableUndoRegistration()

Enables the recording of undo operations.

### Clearing undo operations

func removeAllActions()

Clears the undo and redo stacks and reenables the manager.

