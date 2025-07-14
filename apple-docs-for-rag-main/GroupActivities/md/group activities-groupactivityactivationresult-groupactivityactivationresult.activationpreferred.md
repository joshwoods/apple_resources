

- Group Activities
- GroupActivityActivationResult
-  GroupActivityActivationResult.activationPreferred 

Case

# GroupActivityActivationResult.activationPreferred

A result that indicates the user wants to share the activity with the group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case activationPreferred
```

## Discussion

When you receive this result in your completion handler, call the activate() method of your GroupActivity type to advertise the activity to other participants in the group.

## See Also

### Getting the activation results

case activationDisabled

A result that indicates the user disabled the automatic sharing of activities, or prefers to perform the activity locally.

case cancelled

A result that indicates the user canceled the activation request.

