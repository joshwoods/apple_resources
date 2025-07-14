

- ClassKit
- CLSActivity
-  duration 

Instance Property

# duration

The cumulative time in seconds that an activity has been active.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

When you create a new activity to represent a new attempt at a task by calling the createNewActivity() method, the duration initializes to zero. After you call the start() method, it begins counting seconds. When you call the stop() method, the duration counter stops. It resumes counting (without resetting) if you make a new call to the start() method, enabling you to effectively pause an activity. But once you create a new activity, the duration on the old one stops permanently, and is no longer accessible to your app.

## See Also

### Starting and stopping an activity

func start()

Tells an activity to start recording duration and progress for a task.

func stop()

Tells an activity to stop or pause recording duration and progress for a task.

var isStarted: Bool

A Boolean that indicates whether an activity is running.

