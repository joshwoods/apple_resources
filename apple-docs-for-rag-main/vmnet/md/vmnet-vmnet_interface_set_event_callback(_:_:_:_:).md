

- vmnet
-  vmnet_interface_set_event_callback(\_:\_:\_:\_:) 

Function

# vmnet_interface_set_event_callback(\_:\_:\_:\_:)

Schedules a callback to be executed when events for the specified interface are received.

Mac Catalyst 13.0+macOS 10.10+

``` source
func vmnet_interface_set_event_callback(
    _ interface: interface_ref,
    _ event_mask: interface_event_t,
    _ queue: dispatch_queue_t?,
    _ callback: vmnet_interface_event_callback_t?
) -> vmnet_return_t
```

## Parameters 

`interface`  

The interface reference.

`queue`  

The queue on which the handler is scheduled.

## Return Value

Returns `vmnet` on success, or an error code on failure. See `vmnet` for possible values.

## Discussion

Once the block is set, the callback can be unset by calling the function again, specifying a `NULL` queue and a `NULL` handler.

## See Also

### Starting and Stopping Interfaces

func vmnet_start_interface(xpc_object_t, dispatch_queue_t, vmnet_start_interface_completion_handler_t) -> interface_ref?

Starts host or shared mode on an interface with a specified configuration.

func vmnet_stop_interface(interface_ref, dispatch_queue_t, vmnet_interface_completion_handler_t) -> vmnet_return_t

Stops the interface.

