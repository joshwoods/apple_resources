

- CarKey
- RemoteKeylessEntryAction
-  actionID 

Instance Property

# actionID

The vehicle-specific code that identifies what action to take on the targeted feature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
let actionID: ActionIdentifier
```

## Discussion

You define the action identifiers for your vehicles and what actions they perform on the vehicle function.

## See Also

### Getting the Action Details

let functionID: FunctionIdentifier

The vehicle-specific code that identifies which feature you want to control.

let recipientVehicleID: String

The vehicle to receive the action request.

