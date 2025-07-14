

- XPC
-  xpc_activity_copy_criteria(\_:) 

Function

# xpc_activity_copy_criteria(\_:)

Returns an XPC dictionary that describes the execution criteria of an activity.

macOS 10.9+

``` source
func xpc_activity_copy_criteria(_ activity: xpc_activity_t) -> xpc_object_t?
```

## Discussion

Returns `NULL` in cases where the activity has already completed, for example, when checking in to an event that finished and wasn’t rescheduled.

## See Also

### Execution criteria

func xpc_activity_set_criteria(xpc_activity_t, xpc_object_t)

Modifies the execution criteria of an activity.

