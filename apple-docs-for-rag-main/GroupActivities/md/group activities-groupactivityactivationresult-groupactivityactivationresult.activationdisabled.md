

- Group Activities
- GroupActivityActivationResult
-  GroupActivityActivationResult.activationDisabled 

Case

# GroupActivityActivationResult.activationDisabled

A result that indicates the user disabled the automatic sharing of activities, or prefers to perform the activity locally.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case activationDisabled
```

## Discussion

Use the available context to determine the best way to proceed with this action. For example, instead of sharing a movie with a group, configure playback locally on the user’s device. For activities that only make sense in a group environment, you might alert the user that you can’t start the activity.

## See Also

### Getting the activation results

case activationPreferred

A result that indicates the user wants to share the activity with the group.

case cancelled

A result that indicates the user canceled the activation request.

