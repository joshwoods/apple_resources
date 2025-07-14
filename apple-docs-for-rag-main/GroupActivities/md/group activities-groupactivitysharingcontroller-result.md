

- Group Activities
- GroupActivitySharingController
-  result 

Instance Property

# result

The result of a request to share a group activity.

GroupActivitiesUIKitiOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
@MainActor
var result: GroupActivitySharingResult { get async }
```

## Discussion

Use this property to perform actions related to the starting of the activity. You don’t need to start the activity itself, since the view controller automatically joins your app to the activity when the result is `GroupActivitySharingResult/success`.

## See Also

### Getting the result

enum GroupActivitySharingResult

The result of a request to share a group activity in iOS.

