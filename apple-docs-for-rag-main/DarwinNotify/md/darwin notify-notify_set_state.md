

- Darwin Notify
-  notify_set_state 

Function

# notify_set_state

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
extern uint32_t notify_set_state(int token, uint64_t state64);
```

## Parameters 

`token`  

(Input) notification token

`state64`  

(Input) 64-bit unsigned integer value

## Return Value

Returns status.

## Discussion

Set or get a state value associated with a notification token. Each key in the notification namespace has an associated integer value available for use by clients as for application-specific purposes. A common usage is to allow two processes or threads to synchronize their activities. For example, a server process may need send a notification when a resource becomes available. A client process can register for the notification, but when it starts up it will not know whether the resource is available. The server can set the state value, and the client can check the value at startup time to synchronize with the server.

Set the 64-bit integer state value.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_get_state

notify_post

notify_register_check

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_mach_port

notify_register_signal

notify_resume

notify_suspend

