

- CarKey
- RemoteKeylessEntryAction
-  functionID 

Instance Property

# functionID

The vehicle-specific code that identifies which feature you want to control.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
let functionID: FunctionIdentifier
```

## Discussion

You define the function identifiers for your vehicles and what features they represent.

## See Also

### Getting the Action Details

let actionID: ActionIdentifier

The vehicle-specific code that identifies what action to take on the targeted feature.

let recipientVehicleID: String

The vehicle to receive the action request.

