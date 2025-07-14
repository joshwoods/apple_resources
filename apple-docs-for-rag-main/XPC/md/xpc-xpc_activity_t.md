

- XPC
-  xpc_activity_t 

Type Alias

# xpc_activity_t

An XPC activity object.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_activity_t = xpc_object_t
```

## Discussion

This object represents a set of execution criteria and a current execution state for background activity on the system. After registering an activity, the system evaluates its criteria to determine whether the activity is eligible to run under current system conditions. When an activity becomes eligible to run, its execution state updates and an invocation of its handler block occurs.

## See Also

### Registration

func xpc_activity_register(UnsafePointer&lt;CChar>, xpc_object_t, xpc_activity_handler_t)

Registers an activity with the system.

func xpc_activity_unregister(UnsafePointer&lt;CChar>)

Unregisters an activity with the specified identifier.

let XPC_ACTIVITY_CHECK_IN: xpc_object_t

A constant to check in with the system for a previously registered activity using the same identifier.

typealias xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

