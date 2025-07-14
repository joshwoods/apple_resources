

- ClassKit
- CLSActivity
-  start() 

Instance Method

# start()

Tells an activity to start recording duration and progress for a task.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func start()
```

## Mentioned in 

Recording student progress

## Discussion

Beginning in iOS 11.4, you can start more than one activity at a time, each in its own context. This allows you to nest activities, running a given context and all its ancestors simultaneously, thus measuring progress at multiple levels of context hierarchy concurrently.

## See Also

### Starting and stopping an activity

func stop()

Tells an activity to stop or pause recording duration and progress for a task.

var isStarted: Bool

A Boolean that indicates whether an activity is running.

var duration: TimeInterval

The cumulative time in seconds that an activity has been active.

