

- ClassKit
- CLSDataStore
-  completeAllAssignedActivities(matching:) 

Instance Method

# completeAllAssignedActivities(matching:)

Marks all of the assigned and active activities for the given context path as complete.

iOS 12.2+iPadOS 12.2+Mac Catalyst 12.2+macOS 11.0+visionOS 1.0+

``` source
func completeAllAssignedActivities(matching contextPath: [String])
```

## Parameters 

`contextPath`  

An array of strings that trace a path of identifiers from mainAppContext to a target context with activities you want to mark as complete. The `contextPath` is the same identifier path you use for a call to the contexts(matchingIdentifierPath:completion:) method, but affects only the last context in the path.

## Mentioned in 

Recording student progress

## Discussion

Schoolwork displays a per-student Done indicator to teachers, along with statistics about task completion for the entire class. Students set this indicator in their own view of the Schoolwork app. Use the completeAllAssignedActivities(matching:) method to set the Done status programmatically.

Because you’re taking an action on behalf of the student when you call this method, Schoolwork shows the student a momentary alert in your app’s interface at that time.

Call this method only when you know that the task is complete and the student can’t or won’t work it any further because the task’s allotted time elapsed or because the student submitted all the required information to the teacher. Alternatively, if you already have a submit button in your interface, you can call this method from that button’s handler.

If a teacher reassigns content and the student marks the item done without redoing the activity, ClassKit reports the previously recorded metrics for that assignment to the teacher.

## See Also

### Accessing specific contexts and activities

var mainAppContext: CLSContext

The app’s top-level context.

var activeContext: CLSContext?

The currently active context.

var runningActivity: CLSActivity?

The currently running activity within the currently active context.

func fetchActivity(for: URL, completion: (CLSActivity?, (any Error)?) -> Void)

Fetches an activity for a given document so you can record progress on the associated task.

