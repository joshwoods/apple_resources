

- Darwin Notify
-  notify_check 

Function

# notify_check

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
extern uint32_t notify_check(int token, int * check);
```

## Parameters 

`token`  

(Input) notification token

`check`  

(Output) true/false indication

## Return Value

Returns status.

## Discussion

Check if any notifications have been posted.

Output parameter check is set to 0 for false, 1 for true. Returns status. check is set to true the first time notify_check is called for a token. Subsequent calls set check to true when notifications have been posted for the name associated with the notification token. This routine is independent of notify_post(). That is, check will be true if an application calls notify_post() for a name and then calls notify_check() for a token associated with that name.

## See Also

### Miscellaneous

notify_cancel

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

