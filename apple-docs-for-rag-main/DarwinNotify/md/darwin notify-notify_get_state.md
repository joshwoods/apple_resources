

- Darwin Notify
-  notify_get_state 

Function

# notify_get_state

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
extern uint32_t notify_get_state(int token, uint64_t * state64);
```

## Parameters 

`token`  

(Input) notification token

`state64`  

(Output) 64-bit unsigned integer value

## Return Value

Returns status.

## Discussion

Get the 64-bit integer state value.

## See Also

### Miscellaneous

notify_cancel

notify_check

notify_post

notify_register_check

notify_register_dispatch

Request notification delivery to a dispatch queue.

notify_register_mach_port

notify_register_signal

notify_resume

notify_set_state

notify_suspend

