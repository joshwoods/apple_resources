

- Foundation
- UndoManager
-  enableUndoRegistration() 

Instance Method

# enableUndoRegistration()

Enables the recording of undo operations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enableUndoRegistration()
```

## Discussion

Because undo registration is enabled by default, it is often used to balance a prior disableUndoRegistration() message. Undo registration isn’t actually re-enabled until an enable message balances the last disable message in effect. Raises an `NSInternalInconsistencyException` if invoked while no disableUndoRegistration() message is in effect.

## See Also

### Enabling and disabling undo

func disableUndoRegistration()

Disables the recording of undo operations.

var isUndoRegistrationEnabled: Bool

A Boolean value that indicates whether the recording of undo operations is enabled.

