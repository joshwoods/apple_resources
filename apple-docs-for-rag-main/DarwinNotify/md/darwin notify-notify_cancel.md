

- Darwin Notify
-  notify_cancel 

Function

# notify_cancel

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_cancel(int token);
```

## Parameters 

`token`  

(Input) notification token

## Return Value

Returns status.

## Discussion

Cancel notification and free resources associated with a notification token. Mach ports and file descriptor associated with a token are released (deallocated or closed) when all registration tokens associated with the port or file descriptor have been cancelled.

## See Also

### Miscellaneous

notify_check

notify_get_state

notify_post

notify_register_check

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_mach_port

notify_register_signal

notify_resume

notify_set_state

notify_suspend

