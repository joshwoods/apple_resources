

- ClassKit
- CLSContext
-  currentActivity 

Instance Property

# currentActivity

The activity available for recording progress.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var currentActivity: CLSActivity? { get }
```

## Mentioned in 

Recording student progress

## Discussion

You add an activity to a context by calling the createNewActivity() method when the user makes a new attempt at a task. You then use the context’s currentActivity property to access the newly created activity. If the context has an existing activity from a previous attempt, it ceases to be available to your app as a result of creating a new one. However, the network still retains its data for reporting purposes.

Don’t store a reference to the current activity. Always use the currentActivity property to get it. The object returned to you might change from time to time because of network synchronization, even when the underlying task is the same.

## See Also

### Creating activities

func createNewActivity() -> CLSActivity

Creates and returns a new activity instance for the context.

