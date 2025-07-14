

- XPC
- XPC activities
-  xpc_activity_state_t 

API Collection

# xpc_activity_state_t

A type that represents the state of an activity.

## Overview

An activity is in one of the states that xpc_activity_state_t defines. Apps may check the current state of the activity using xpc_activity_get_state(_:) in the handler block that you provide to xpc_activity_register(_:_:_:).

The app can modify the state of the activity by calling xpc_activity_set_state(_:_:) with one of the following:

- XPC_ACTIVITY_STATE_DEFER

- XPC_ACTIVITY_STATE_CONTINUE

- XPC_ACTIVITY_STATE_DONE

## Topics

### Constants

var XPC_ACTIVITY_STATE_CHECK_IN: Int

The activity has completed a check-in with the system.

var XPC_ACTIVITY_STATE_CONTINUE: Int

The activity continues its operation beyond the return of its handler block.

var XPC_ACTIVITY_STATE_DEFER: Int

The activity needs to wait until it satisfies its criteria again.

var XPC_ACTIVITY_STATE_DONE: Int

The activity is complete.

var XPC_ACTIVITY_STATE_RUN: Int

The activity is eligible to run according to its criteria.

var XPC_ACTIVITY_STATE_WAIT: Int

The activity is waiting for an opportunity to run.

## See Also

### State

func xpc_activity_get_state(xpc_activity_t) -> xpc_activity_state_t

Returns the current state of an activity.

func xpc_activity_set_state(xpc_activity_t, xpc_activity_state_t) -> Bool

Updates the current state of an activity.

func xpc_activity_should_defer(xpc_activity_t) -> Bool

Tests whether to defer an activity.

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

