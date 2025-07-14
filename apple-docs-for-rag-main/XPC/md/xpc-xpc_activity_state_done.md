

- XPC
-  XPC_ACTIVITY_STATE_DONE 

Global Variable

# XPC_ACTIVITY_STATE_DONE

The activity is complete.

iOSiPadOSMac CatalystmacOS

``` source
var XPC_ACTIVITY_STATE_DONE: Int { get }
```

## Discussion

An app may pass this value to xpc_activity_set_state(_:_:) to indicate when the activity completes. For nonrepeating activity, the resources for the activity automatically release upon return from the handler block. For repeating activity, timers present in the activity’s criteria reset.

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

var XPC_ACTIVITY_STATE_WAIT: Int

The activity is waiting for an opportunity to run.

var XPC_ACTIVITY_STATE_RUN: Int

The activity is eligible to run according to its criteria.

var XPC_ACTIVITY_STATE_DEFER: Int

The activity needs to wait until it satisfies its criteria again.

var XPC_ACTIVITY_STATE_CONTINUE: Int

The activity continues its operation beyond the return of its handler block.

