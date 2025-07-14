

- ClassKit
- CLSContext
-  createNewActivity() 

Instance Method

# createNewActivity()

Creates and returns a new activity instance for the context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func createNewActivity() -> CLSActivity
```

## Return Value

A new activity.

## Mentioned in 

Recording student progress

## Discussion

Use this method to create a new activity for a context every time the user makes a new attempt at a task. Afterward, you can use the returned value, or retrieve it by accessing the context’s currentActivity property. However, don’t store a reference to the activity as a class property, because the underlying object may change from time to time as the framework performs network synchronization.

When you call this method on a context that already has an activity, the old activity is stopped and ceases to be accessible to your app, although its data remains in the network.

## See Also

### Creating activities

var currentActivity: CLSActivity?

The activity available for recording progress.

