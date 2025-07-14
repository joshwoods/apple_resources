

- Foundation
- ProcessInfo
-  ProcessInfo.ActivityOptions 

Structure

# ProcessInfo.ActivityOptions

Option flags used with beginActivity(options:reason:) and performActivity(options:reason:using:).

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ActivityOptions
```

## Overview

To include one of these individual flags in one of the sets, use bitwise `OR`; for example, during a presentation you might use:

```
NSActivityUserInitiated | NSActivityIdleDisplaySleepDisabled
```

To exclude from one of the sets, use bitwise `AND` with `NOT`; for example, during a user initiated action that may be safely terminated with no application interaction in case of logout you might use:

```
NSActivityUserInitiated & ~NSActivitySuddenTerminationDisabled
```

## Topics

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

static var trackingEnabled: ProcessInfo.ActivityOptions

A flag to track the activity with a signpost interval.

### Initializers

init(rawValue: UInt64)

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

static var trackingEnabled: ProcessInfo.ActivityOptions

A flag to track the activity with a signpost interval.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

struct OperatingSystemVersion

A structure that contains version information about the currently executing operating system, including major, minor, and patch version numbers.

enum ThermalState

Values used to indicate the system’s thermal state.

Anonymous

The following constants are provided by the `NSProcessInfo` class as return values for operatingSystem().

