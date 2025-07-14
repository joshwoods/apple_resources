

- Darwin Notify
-  notify_register_check 

Function

# notify_register_check

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_register_check(const char * name, int * out_token);
```

## Parameters 

`name`  

(Input) notification name

`out_token`  

(Output) registration token

## Return Value

Returns status.

## Discussion

Creates a registration token be used with notify_check(), but no active notifications will be delivered.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_get_state

notify_post

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_mach_port

notify_register_signal

notify_resume

notify_set_state

notify_suspend

