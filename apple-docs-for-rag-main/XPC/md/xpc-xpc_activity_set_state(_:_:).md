

- XPC
-  xpc_activity_set_state(\_:\_:) 

Function

# xpc_activity_set_state(\_:\_:)

Updates the current state of an activity.

macOS 10.9+

``` source
func xpc_activity_set_state(
    _ activity: xpc_activity_t,
    _ state: xpc_activity_state_t
) -> Bool
```

## Return Value

Returns `true` if the state was successfully updated; otherwise, returns `false` if the requested state transition is not valid.

## See Also

### State

func xpc_activity_get_state(xpc_activity_t) -> xpc_activity_state_t

Returns the current state of an activity.

func xpc_activity_should_defer(xpc_activity_t) -> Bool

Tests whether to defer an activity.

xpc_activity_state_t

A type that represents the state of an activity.

typealias xpc_activity_state_t

A type that represents the state of an activity.

var XPC_ACTIVITY_STATE_CHECK_IN: Int

The activity has completed a check-in with the system.

var XPC_ACTIVITY_STATE_WAIT: Int

The activity is waiting for an opportunity to run.

var XPC_ACTIVITY_STATE_RUN: Int

The activity is eligible to run according to its criteria.

var XPC_ACTIVITY_STATE_DEFER: Int

The activity needs to wait until it satisfies its criteria again.

var XPC_ACTIVITY_STATE_CONTINUE: Int

The activity continues its operation beyond the return of its handler block.

var XPC_ACTIVITY_STATE_DONE: Int

The activity is complete.

