

- CarKey
- RemoteKeylessEntryEnduringAction
-  actionID Deprecated

Instance Property

# actionID

The vehicle-specific code that identifies what action to take on the targeted feature.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
let actionID: ActionIdentifier
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Discussion

You define the action identifiers for your vehicles and what actions they perform on the vehicle function.

## See Also

### Getting the Action Details

let functionID: FunctionIdentifier

The vehicle-specific code that identifies which feature you want to control.

Deprecated

let recipientVehicleID: String

The vehicle to receive the action request.

Deprecated

