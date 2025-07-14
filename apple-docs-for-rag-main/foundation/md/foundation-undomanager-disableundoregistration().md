

- Foundation
- UndoManager
-  disableUndoRegistration() 

Instance Method

# disableUndoRegistration()

Disables the recording of undo operations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func disableUndoRegistration()
```

## Discussion

This method disables undos recorded by registerUndo(withTarget:selector:object:) or invocation-based undo.

This method can be invoked multiple times by multiple clients. The enableUndoRegistration() method must be invoked an equal number of times to re-enable undo registration.

## See Also

### Enabling and disabling undo

func enableUndoRegistration()

Enables the recording of undo operations.

var isUndoRegistrationEnabled: Bool

A Boolean value that indicates whether the recording of undo operations is enabled.

