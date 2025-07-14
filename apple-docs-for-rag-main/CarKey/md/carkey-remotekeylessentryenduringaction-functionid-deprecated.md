

- CarKey
- RemoteKeylessEntryEnduringAction
-  functionID Deprecated

Instance Property

# functionID

The vehicle-specific code that identifies which feature you want to control.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
let functionID: FunctionIdentifier
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Discussion

You define the function identifiers for your vehicles and what features they represent.

## See Also

### Getting the Action Details

let actionID: ActionIdentifier

The vehicle-specific code that identifies what action to take on the targeted feature.

Deprecated

let recipientVehicleID: String

The vehicle to receive the action request.

Deprecated

