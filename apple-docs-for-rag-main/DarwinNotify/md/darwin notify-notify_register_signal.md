

- Darwin Notify
-  notify_register_signal 

Function

# notify_register_signal

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_register_signal(const char * name, int sig, int * out_token);
```

## Parameters 

`name`  

(Input) notification name

`sig`  

(Input) signal number (see signal(3))

`out_token`  

(Output) notification token

## Return Value

Returns status.

## Discussion

Request notification delivery by UNIX signal.

A client may request signal notification for multiple names. After a signal is delivered, the notify_check() routine may be called with each notification token to determine which name (if any) generated the signal notification.

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

notify_resume

notify_set_state

notify_suspend

