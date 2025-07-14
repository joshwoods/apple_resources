

- Darwin Notify
-  notify_resume 

Function

# notify_resume

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
extern uint32_t notify_resume(int token);
```

## Parameters 

`token`  

(Input) notification token

## Return Value

Returns status.

## Discussion

Removes one level of suspension for a token previously suspended by a call to notify_suspend. Notifications will resume when a matching call to notify_resume is made for each previous call to notify_suspend. Notifications posted while a token is suspended are coalesced into a single notification sent following a resumption.

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

notify_set_state

notify_suspend

