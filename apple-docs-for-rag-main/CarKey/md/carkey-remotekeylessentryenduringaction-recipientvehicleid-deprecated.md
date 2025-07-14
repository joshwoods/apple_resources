

- CarKey
- RemoteKeylessEntryEnduringAction
-  recipientVehicleID Deprecated

Instance Property

# recipientVehicleID

The vehicle to receive the action request.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
let recipientVehicleID: String
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Discussion

This string is the same one that appears in the identifier property of one of the session’s vehicle reports.

## See Also

### Getting the Action Details

let functionID: FunctionIdentifier

The vehicle-specific code that identifies which feature you want to control.

Deprecated

let actionID: ActionIdentifier

The vehicle-specific code that identifies what action to take on the targeted feature.

Deprecated

