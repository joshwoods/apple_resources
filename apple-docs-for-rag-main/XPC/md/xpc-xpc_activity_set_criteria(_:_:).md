

- XPC
-  xpc_activity_set_criteria(\_:\_:) 

Function

# xpc_activity_set_criteria(\_:\_:)

Modifies the execution criteria of an activity.

macOS 10.9+

``` source
func xpc_activity_set_criteria(
    _ activity: xpc_activity_t,
    _ criteria: xpc_object_t
)
```

## See Also

### Execution criteria

func xpc_activity_copy_criteria(xpc_activity_t) -> xpc_object_t?

Returns an XPC dictionary that describes the execution criteria of an activity.

