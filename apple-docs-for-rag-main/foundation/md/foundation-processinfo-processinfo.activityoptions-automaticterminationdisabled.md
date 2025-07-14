

- Foundation
- ProcessInfo
- ProcessInfo.ActivityOptions
-  automaticTerminationDisabled 

Type Property

# automaticTerminationDisabled

A flag to prevent automatic termination.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var automaticTerminationDisabled: ProcessInfo.ActivityOptions { get }
```

## Discussion

This is included by userInitiatedAllowingIdleSystemSleep.

## See Also

### Constants

static var idleDisplaySleepDisabled: ProcessInfo.ActivityOptions

A flag to require the screen to stay powered on.

static var idleSystemSleepDisabled: ProcessInfo.ActivityOptions

A flag to prevent idle sleep.

static var suddenTerminationDisabled: ProcessInfo.ActivityOptions

A flag to prevent sudden termination.

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

static var trackingEnabled: ProcessInfo.ActivityOptions

A flag to track the activity with a signpost interval.

