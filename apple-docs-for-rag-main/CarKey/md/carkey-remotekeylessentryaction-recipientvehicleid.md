

- CarKey
- RemoteKeylessEntryAction
-  recipientVehicleID 

Instance Property

# recipientVehicleID

The vehicle to receive the action request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
let recipientVehicleID: String
```

## Discussion

This string is the same one that appears in the identifier property of one of the session’s vehicle reports.

## See Also

### Getting the Action Details

let functionID: FunctionIdentifier

The vehicle-specific code that identifies which feature you want to control.

let actionID: ActionIdentifier

The vehicle-specific code that identifies what action to take on the targeted feature.

