

- Group Activities
- GroupActivitySharingController
-  init(\_:) 

Initializer

# init(\_:)

Initializes the sharing controller with the specified activity and type information.

GroupActivitiesUIKitiOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
@MainActor
init(_ activity: ActivityType) throws where ActivityType : GroupActivity
```

## Parameters 

`activity`  

The activity object to start.

## See Also

### Creating the group activity sharing controller

init&lt;ActivityType>(preparationHandler: () async throws -> ActivityType)

Initializes the SharePlay sharing controller with a closure that creates the activity object.

