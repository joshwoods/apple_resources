

- Darwin Notify
-  notify_suspend 

Function

# notify_suspend

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
extern uint32_t notify_suspend(int token);
```

## Parameters 

`token`  

(Input) notification token

## Return Value

Returns status.

## Discussion

Suspend delivery of notifications for a token. Notifications for this token will be pended and coalesced, then delivered following a matching call to notify_resume. Calls to notify_suspend may be nested. Notifications remain suspended until an equal number of calls have been made to notify_resume.

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

notify_set_state

