

- XPC
-  XPC_ACTIVITY_CHECK_IN 

Global Variable

# XPC_ACTIVITY_CHECK_IN

A constant to check in with the system for a previously registered activity using the same identifier.

macOS 10.9+

``` source
let XPC_ACTIVITY_CHECK_IN: xpc_object_t
```

## Discussion

Pass this constant to xpc_activity_register(_:_:_:) as the criteria dictionary to check in with the system for previously registered activity using the same identifier (for example, an activity from a launchd property list).

## See Also

### Registration

func xpc_activity_register(UnsafePointer&lt;CChar>, xpc_object_t, xpc_activity_handler_t)

Registers an activity with the system.

func xpc_activity_unregister(UnsafePointer&lt;CChar>)

Unregisters an activity with the specified identifier.

typealias xpc_activity_t

An XPC activity object.

typealias xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

