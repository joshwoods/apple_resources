

- Darwin Notify
-  notify_register_dispatch 

Function

# notify_register_dispatch

Request notification delivery to a dispatch queue.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
extern uint32_t notify_register_dispatch(const char * name, int * out_token, dispatch_queue_t queue, notify_handler_thandler);
```

## Parameters 

`name`  

(Input) The notification name.

`out_token`  

(Output) The registration token.

`queue`  

(Input) The dispatch queue to which the Block is submitted. The dispatch queue is retained by the notify subsystem while the notification is registered, and will be released when notification is canceled.

`handler`  

(Input) The Block to invoke on the dispatch queue in response to a notification. The notification token is passed to the Block as an argument so that the callee can modify the state of the notification or cancel the registration.

## Return Value

Returns status.

## Discussion

When notifications are received by the process, the notify subsystem will deliver the registered Block to the target dispatch queue. Notification blocks are not re-entrant, and subsequent notification Blocks will not be delivered for the same registration until the previous Block has returned.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_get_state

notify_post

notify_register_check

notify_register_mach_port

notify_register_signal

notify_resume

notify_set_state

notify_suspend

