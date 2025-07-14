

- Foundation
- ProcessInfo
- ProcessInfo.ActivityOptions
-  trackingEnabled 

Type Property

# trackingEnabled

A flag to track the activity with a signpost interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var trackingEnabled: ProcessInfo.ActivityOptions { get }
```

## Discussion

To help you investigate perfomance issues in your app, use trackingEnabled to track the timing of a user interaction by annotating the beginning and end of an activity using a signpost interval.

Calling beginActivity(options:reason:) to begin the activity returns an object token that you retain for the duration of the activity. The logging system produces a distinct message, useful in debugging, if the object token is de-allocated before you call endActivity(_:).

The flag trackingEnabled differs from animationTrackingEnabled in the type of interval signposts the logging system emits. Use animationTrackingEnabled when the interaction involves an animation.

## See Also

### Related Documentation

Recording Performance Data

Add signposts to record interesting time-based events.

### Constants

static var idleDisplaySleepDisabled: ProcessInfo.ActivityOptions

A flag to require the screen to stay powered on.

static var idleSystemSleepDisabled: ProcessInfo.ActivityOptions

A flag to prevent idle sleep.

static var suddenTerminationDisabled: ProcessInfo.ActivityOptions

A flag to prevent sudden termination.

static var automaticTerminationDisabled: ProcessInfo.ActivityOptions

A flag to prevent automatic termination.

static var userInitiated: ProcessInfo.ActivityOptions

A flag to indicate the app is performing a user-requested action.

static var userInteractive: ProcessInfo.ActivityOptions

A flag to indicate the app is responding to user interaction.

static var userInitiatedAllowingIdleSystemSleep: ProcessInfo.ActivityOptions

A flag to indicate the app is performing a user-requested action, but that the system can sleep on idle.

static var background: ProcessInfo.ActivityOptions

A flag to indicate the app has initiated some kind of work, but not as the direct result of user request.

static var latencyCritical: ProcessInfo.ActivityOptions

A flag to indicate the activity requires the highest amount of timer and I/O precision available.

static var animationTrackingEnabled: ProcessInfo.ActivityOptions

A flag to track the activity with an animation signpost interval.

