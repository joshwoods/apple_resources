

- ClassKit
- CLSDataStore
-  mainAppContext 

Instance Property

# mainAppContext

The app’s top-level context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var mainAppContext: CLSContext { get }
```

## Discussion

Every app has exactly one top-level context that acts as the root node in a hierarchy of contexts that you define. Its identifier is the app’s bundle identifier. You can neither create nor destroy this context.

## See Also

### Accessing specific contexts and activities

var activeContext: CLSContext?

The currently active context.

var runningActivity: CLSActivity?

The currently running activity within the currently active context.

func fetchActivity(for: URL, completion: (CLSActivity?, (any Error)?) -> Void)

Fetches an activity for a given document so you can record progress on the associated task.

func completeAllAssignedActivities(matching: [String])

Marks all of the assigned and active activities for the given context path as complete.

