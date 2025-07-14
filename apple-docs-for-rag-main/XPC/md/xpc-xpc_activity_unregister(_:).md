

- XPC
-  xpc_activity_unregister(\_:) 

Function

# xpc_activity_unregister(\_:)

Unregisters an activity with the specified identifier.

macOS 10.9+

``` source
func xpc_activity_unregister(_ identifier: UnsafePointer)
```

## Parameters 

`identifier`  

The identifier of the activity to unregister.

## Discussion

A dynamically registered activity will be deleted in response to this call. Statically registered activity (from a launchd property list) will be reverted to its original criteria if any modifications were made.

Unregistering an activity has no effect on any outstanding xpc_activity_t objects or any currently executing xpc_activity_handler_t blocks; however, no new handler block invocations will be made after it is unregistered.

## See Also

### Registration

func xpc_activity_register(UnsafePointer&lt;CChar>, xpc_object_t, xpc_activity_handler_t)

Registers an activity with the system.

let XPC_ACTIVITY_CHECK_IN: xpc_object_t

A constant to check in with the system for a previously registered activity using the same identifier.

typealias xpc_activity_t

An XPC activity object.

typealias xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

