

- ClassKit
- CLSDataStore
-  runningActivity 

Instance Property

# runningActivity

The currently running activity within the currently active context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var runningActivity: CLSActivity? { get }
```

## Mentioned in 

Recording student progress

## Discussion

This value is `nil` if there is no currently running activity.

If your deployment target is iOS 11.4 or later, you can have more than one activity running concurrently. When you do this, the runningActivity property holds the most recently started activity.

## See Also

### Accessing specific contexts and activities

var mainAppContext: CLSContext

The app’s top-level context.

var activeContext: CLSContext?

The currently active context.

func fetchActivity(for: URL, completion: (CLSActivity?, (any Error)?) -> Void)

Fetches an activity for a given document so you can record progress on the associated task.

func completeAllAssignedActivities(matching: [String])

Marks all of the assigned and active activities for the given context path as complete.

