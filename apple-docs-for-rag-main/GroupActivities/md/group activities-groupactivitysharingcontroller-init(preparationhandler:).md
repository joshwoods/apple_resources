

- Group Activities
- GroupActivitySharingController
-  init(preparationHandler:) 

Initializer

# init(preparationHandler:)

Initializes the SharePlay sharing controller with a closure that creates the activity object.

GroupActivitiesUIKitiOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
@MainActor
init(preparationHandler: @escaping () async throws -> ActivityType) where ActivityType : GroupActivity
```

## Parameters 

`preparationHandler`  

A closure that takes no parameters and returns the activity object.

## Discussion

The initializer executes the closure asynchronously so that your app can present the view controller in a timely manner. Use this method when the creation of the GroupActivity object might take a significant amount of time.

## See Also

### Creating the group activity sharing controller

init&lt;ActivityType>(ActivityType) throws

Initializes the sharing controller with the specified activity and type information.

