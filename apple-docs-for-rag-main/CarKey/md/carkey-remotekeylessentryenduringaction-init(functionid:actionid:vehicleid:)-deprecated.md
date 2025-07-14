

- CarKey
- RemoteKeylessEntryEnduringAction
-  init(functionID:actionID:vehicleID:) Deprecated

Initializer

# init(functionID:actionID:vehicleID:)

Creates a new action object with the specified action-specific details and vehicle ID.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
init(
    functionID: FunctionIdentifier,
    actionID: ActionIdentifier,
    vehicleID: String
)
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Parameters 

`functionID`  

The vehicle-specific code that identifies the feature to activate. For example, the vehicle might have a specific code to identify the roof mechanism on a convertible vehicle.

`actionID`  

The vehicle-specific code that defines what action to take on the vehicle feature. For example, a vehicle might have separate actions to raise or lower the top on a convertible.

`vehicleID`  

The target vehicle for the action. Choose the vehicle from one of the session’s vehicle reports. Specify the string in the identifier property of the corresponding report.

## Return Value

An enduring action object with the specified information.

## Discussion

This method creates an immutable action object that you can pass to your session’s perform(_:) method.

