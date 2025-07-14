

- Darwin Notify
-  notify_register_mach_port 

Function

# notify_register_mach_port

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_register_mach_port(const char * name, mach_port_t * notify_port, int flags, int * out_token);
```

## Parameters 

`name`  

(Input) notification name

`notify_port`  

(Input/Output) pointer to a mach port

`out_token`  

(Output) notification token

## Return Value

Returns status.

## Discussion

Request notification by mach message.

Notifications are delivered by an empty message sent to a mach port. By default, a new port is allocated and a pointer to it is returned as the value of “notify_port”. A mach port previously returned by a call to this routine may be used for notifications if a pointer to that port is passed in to the routine and NOTIFY_REUSE is set in the flags parameter. The notification service must be able to extract send rights to the port.

Note that the kernel limits the size of the message queue for any port. If it is important that notifications should not be lost due to queue overflow, clients should service messages quickly, and be careful about using the same port for notifications for more than one name.

A notification message has an empty message body. The msgh_id field in the mach message header will have the value of the notification token. If a port is reused for multiple notification registrations, the msgh_id value may be used to determine which name generated the notification.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_get_state

notify_post

notify_register_check

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_signal

notify_resume

notify_set_state

notify_suspend

