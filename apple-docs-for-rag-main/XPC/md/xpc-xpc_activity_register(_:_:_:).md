

- XPC
-  xpc_activity_register(\_:\_:\_:) 

Function

# xpc_activity_register(\_:\_:\_:)

Registers an activity with the system.

macOS 10.9+

``` source
func xpc_activity_register(
    _ identifier: UnsafePointer,
    _ criteria: xpc_object_t,
    _ handler: @escaping xpc_activity_handler_t
)
```

## Parameters 

`identifier`  

A unique identifier for the activity. Each application has its own namespace.

`criteria`  

A dictionary of criteria for the activity.

`handler`  

The handler block to be called when the activity changes state to one of the following states:

- XPC_ACTIVITY_STATE_CHECK_IN (optional)

- XPC_ACTIVITY_STATE_RUN

The handler block is never invoked reentrantly. It will be invoked on a dispatch queue with an appropriate priority to perform the activity.

## Discussion

Registers a new activity with the system. The criteria of the activity are described by the dictionary passed to this function. If an activity with the same identifier already exists, the criteria provided override the existing criteria unless the special dictionary XPC_ACTIVITY_CHECK_IN is used. The XPC_ACTIVITY_CHECK_IN dictionary instructs the system to first look up an existing activity without modifying its criteria. Once the existing activity is found (or a new one is created with an empty set of criteria) the handler will be called with an activity object in the XPC_ACTIVITY_STATE_CHECK_IN state.

## See Also

### Registration

func xpc_activity_unregister(UnsafePointer&lt;CChar>)

Unregisters an activity with the specified identifier.

let XPC_ACTIVITY_CHECK_IN: xpc_object_t

A constant to check in with the system for a previously registered activity using the same identifier.

typealias xpc_activity_t

An XPC activity object.

typealias xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

