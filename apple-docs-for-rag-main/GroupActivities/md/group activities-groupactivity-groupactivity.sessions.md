

- Group Activities
- GroupActivity
-  GroupActivity.Sessions 

Type Alias

# GroupActivity.Sessions

A type that provides asynchronous, sequential, iterated access to the sessions for the activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
typealias Sessions = GroupSession.Sessions
```

## Discussion

A `Sessions` type contains a sequence of GroupSession objects specific to the current activity. The sessions() method returns this type, and you use it to retrieve the current session, if any, for that activity. The system creates only one GroupSession object for each new activity. To detect changes to the session’s state, activity type, or active participants, subscribe to the corresponding properties.

## See Also

### Receiving an activity-related session

static func sessions() -> Self.Sessions

Returns the sessions for this activity as an asynchronous sequence.

