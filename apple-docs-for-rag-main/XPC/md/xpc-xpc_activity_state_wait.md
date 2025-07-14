

- XPC
-  XPC_ACTIVITY_STATE_WAIT 

Global Variable

# XPC_ACTIVITY_STATE_WAIT

The activity is waiting for an opportunity to run.

iOSiPadOSMac CatalystmacOS

``` source
var XPC_ACTIVITY_STATE_WAIT: Int { get }
```

## Discussion

This value never returns within the activity’s handler block because the block’s invocation is in response to XPC_ACTIVITY_STATE_CHECK_IN or XPC_ACTIVITY_STATE_RUN.

A launchd job may idle exit while an activity is in the wait state and relaunch in response to the activity becoming runnable. The launchd job simply needs to reregister for the activity on its next launch by passing XPC_ACTIVITY_STATE_CHECK_IN to xpc_activity_register(_:_:_:).

## See Also

### State

func xpc_activity_get_state(xpc_activity_t) -> xpc_activity_state_t

Returns the current state of an activity.

func xpc_activity_set_state(xpc_activity_t, xpc_activity_state_t) -> Bool

Updates the current state of an activity.

func xpc_activity_should_defer(xpc_activity_t) -> Bool

Tests whether to defer an activity.

xpc_activity_state_t

A type that represents the state of an activity.

typealias xpc_activity_state_t

A type that represents the state of an activity.

var XPC_ACTIVITY_STATE_CHECK_IN: Int

The activity has completed a check-in with the system.

var XPC_ACTIVITY_STATE_RUN: Int

The activity is eligible to run according to its criteria.

var XPC_ACTIVITY_STATE_DEFER: Int

The activity needs to wait until it satisfies its criteria again.

var XPC_ACTIVITY_STATE_CONTINUE: Int

The activity continues its operation beyond the return of its handler block.

var XPC_ACTIVITY_STATE_DONE: Int

The activity is complete.

