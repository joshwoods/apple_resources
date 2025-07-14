

- RealityKit
- ActionEventType
-  updated 

Type Property

# updated

An event that takes place after an action event starts and is within its time interval.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static var updated: ActionEventType { get }
```

## See Also

### Event types

static var started: ActionEventType

An event that takes place when a new action event begins.

static var ended: ActionEventType

An event that takes place when the action event exits its time interval.

static var paused: ActionEventType

An event that takes place when the animation pauses.

static var resumed: ActionEventType

An event that takes place when the animation resumes after a pause.

static var skipped: ActionEventType

An event that takes place when the system misses an action event’s time interval.

static var terminated: ActionEventType

An event that takes place when the animation ends.

