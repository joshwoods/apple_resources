

- Darwin Notify
-  notify_post 

Function

# notify_post

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_post(const char * name);
```

## Discussion

Post a notification for a name.

This is the only call that is required for a notification producer. Returns status.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_get_state

notify_register_check

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_mach_port

notify_register_signal

notify_resume

notify_set_state

notify_suspend

