

- Dispatch
-  dispatch_get_current_queue() 

Function

# dispatch_get_current_queue()

Returns the queue on which the currently executing block is running.

tvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func dispatch_get_current_queue() -> dispatch_queue_t
```

## Return Value

Returns the current queue.

## Discussion

This function is defined to never return `NULL`.

When called from outside of the context of a submitted block, this function returns the main queue if the call is executed from the main thread. If the call is made from any other thread, this function returns the default concurrent queue.

## See Also

### Functions

func dispatch_debugv(dispatch_object_t, UnsafePointer&lt;CChar>, CVaListPointer)

