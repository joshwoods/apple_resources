

- ClassKit
- CLSActivity
-  isStarted 

Instance Property

# isStarted

A Boolean that indicates whether an activity is running.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var isStarted: Bool { get }
```

## See Also

### Starting and stopping an activity

func start()

Tells an activity to start recording duration and progress for a task.

func stop()

Tells an activity to stop or pause recording duration and progress for a task.

var duration: TimeInterval

The cumulative time in seconds that an activity has been active.

