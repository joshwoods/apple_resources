

- XPC
-  xpc_activity_handler_t 

Type Alias

# xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_activity_handler_t = (xpc_activity_t) -> Void
```

## See Also

### Registration

func xpc_activity_register(UnsafePointer&lt;CChar>, xpc_object_t, xpc_activity_handler_t)

Registers an activity with the system.

func xpc_activity_unregister(UnsafePointer&lt;CChar>)

Unregisters an activity with the specified identifier.

let XPC_ACTIVITY_CHECK_IN: xpc_object_t

A constant to check in with the system for a previously registered activity using the same identifier.

typealias xpc_activity_t

An XPC activity object.

