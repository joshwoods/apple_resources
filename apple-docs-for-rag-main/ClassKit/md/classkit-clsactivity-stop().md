

- ClassKit
- CLSActivity
-  stop() 

Instance Method

# stop()

Tells an activity to stop or pause recording duration and progress for a task.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func stop()
```

## Mentioned in 

Recording student progress

Recording additional metrics about a completed task

## Discussion

If your app uses this method to pause recording, such as when the user taps the pause button in a game, you can resume later with another call to start() on the same activity when the user resumes the task associated with the activity. But if the user makes a new attempt at the task, for example by starting a game level over, and your app creates a new activity with a call to createNewActivity(), then the framework stops the old one permanently and makes it inaccessible to your app thereafter.

## See Also

### Starting and stopping an activity

func start()

Tells an activity to start recording duration and progress for a task.

var isStarted: Bool

A Boolean that indicates whether an activity is running.

var duration: TimeInterval

The cumulative time in seconds that an activity has been active.

