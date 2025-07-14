

- XPC
-  XPC activities 

API Collection

# XPC activities

Schedule background activities for the system to execute.

## Topics

### Registration

func xpc_activity_register(UnsafePointer&lt;CChar>, xpc_object_t, xpc_activity_handler_t)

Registers an activity with the system.

func xpc_activity_unregister(UnsafePointer&lt;CChar>)

Unregisters an activity with the specified identifier.

let XPC_ACTIVITY_CHECK_IN: xpc_object_t

A constant to check in with the system for a previously registered activity using the same identifier.

typealias xpc_activity_t

An XPC activity object.

typealias xpc_activity_handler_t

A block to call when an XPC activity becomes eligible to run.

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

var XPC_ACTIVITY_STATE_DONE: Int

The activity is complete.

### Execution criteria

func xpc_activity_copy_criteria(xpc_activity_t) -> xpc_object_t?

Returns an XPC dictionary that describes the execution criteria of an activity.

func xpc_activity_set_criteria(xpc_activity_t, xpc_object_t)

Modifies the execution criteria of an activity.

### Scheduling

let XPC_ACTIVITY_REPEATING: UnsafePointer&lt;CChar>

A Boolean property that indicates whether this is a repeating activity.

let XPC_ACTIVITY_DELAY: UnsafePointer&lt;CChar>

An integer property that indicates the number of seconds to delay before beginning the activity.

let XPC_ACTIVITY_GRACE_PERIOD: UnsafePointer&lt;CChar>

An integer property that indicates the number of seconds to allow as a grace period before the scheduling of the activity becomes more aggressive.

### Time Intervals

let XPC_ACTIVITY_INTERVAL: UnsafePointer&lt;CChar>

An integer property that indicates the desired time interval of the activity in seconds.

let XPC_ACTIVITY_INTERVAL_1_MIN: Int64

A constant that represents a 1-minute time interval.

let XPC_ACTIVITY_INTERVAL_5_MIN: Int64

A constant that represents a 5-minute time interval.

let XPC_ACTIVITY_INTERVAL_15_MIN: Int64

A constant that represents a 15-minute time interval.

let XPC_ACTIVITY_INTERVAL_30_MIN: Int64

A constant that represents a 30-minute time interval.

let XPC_ACTIVITY_INTERVAL_1_HOUR: Int64

A constant that represents a 1-hour time interval.

let XPC_ACTIVITY_INTERVAL_4_HOURS: Int64

A constant that represents a 4-hour time interval.

let XPC_ACTIVITY_INTERVAL_8_HOURS: Int64

A constant that represents an 8-hour time interval.

let XPC_ACTIVITY_INTERVAL_1_DAY: Int64

A constant that represents a one-day time interval.

let XPC_ACTIVITY_INTERVAL_7_DAYS: Int64

A constant that represents a seven-day time interval.

### Priority

let XPC_ACTIVITY_PRIORITY: UnsafePointer&lt;CChar>

A string property that indicates the priority of the activity.

let XPC_ACTIVITY_PRIORITY_MAINTENANCE: UnsafePointer&lt;CChar>

A string that indicates an activity is maintenance priority.

let XPC_ACTIVITY_PRIORITY_UTILITY: UnsafePointer&lt;CChar>

A string that indicates an activity is utility priority.

### Power consumption

let XPC_ACTIVITY_ALLOW_BATTERY: UnsafePointer&lt;CChar>

A Boolean value that indicates whether to allow the activity to run while the computer is on battery power.

let XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP: UnsafePointer&lt;CChar>

A Boolean value that indicates whether the activity performs only while the primary screen is in sleep mode.

let XPC_ACTIVITY_PREVENT_DEVICE_SLEEP: UnsafePointer&lt;CChar>

A Boolean that indicates whether the activity prevents the system from sleeping while on battery power.

