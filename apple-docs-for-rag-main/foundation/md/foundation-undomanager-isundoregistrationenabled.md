

- Foundation
- UndoManager
-  isUndoRegistrationEnabled 

Instance Property

# isUndoRegistrationEnabled

A Boolean value that indicates whether the recording of undo operations is enabled.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isUndoRegistrationEnabled: Bool { get }
```

## Discussion

true if registration is enabled; otherwise, false.

The default is true.

## See Also

### Enabling and disabling undo

func disableUndoRegistration()

Disables the recording of undo operations.

func enableUndoRegistration()

Enables the recording of undo operations.

