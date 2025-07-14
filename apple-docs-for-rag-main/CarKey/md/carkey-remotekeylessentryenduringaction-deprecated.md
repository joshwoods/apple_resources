

- CarKey
-  RemoteKeylessEntryEnduringAction Deprecated

Structure

# RemoteKeylessEntryEnduringAction

An action with an optional stopping point that you want to perform on a vehicle.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
struct RemoteKeylessEntryEnduringAction
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Overview

Use a RemoteKeylessEntryEnduringAction object to store details about an action that you can stop or let run to completion. For example, you might use this type of action to lower or raise the top of a convertible vehicle. The object stores information about the vehicle feature to control and the action to take on that feature. It also stores the identifier for the vehicle itself.

After you create a RemoteKeylessEntryEnduringAction object, call your session’s perform(_:) method to execute the action. Use the returned RemoteKeylessEntryAction.ExecutionRequest object to determine the success or failure of the request.

## Topics

### Creating the Action Request

init(functionID: FunctionIdentifier, actionID: ActionIdentifier, vehicleID: String)

Creates a new action object with the specified action-specific details and vehicle ID.

### Receiving the Action’s Response

class EnduringExecutionRequest

An object that reports the results of an action with an optional stopping point.

### Getting the Action Details

let functionID: FunctionIdentifier

The vehicle-specific code that identifies which feature you want to control.

let actionID: ActionIdentifier

The vehicle-specific code that identifies what action to take on the targeted feature.

let recipientVehicleID: String

The vehicle to receive the action request.

## See Also

### Vehicle Actions

struct RemoteKeylessEntryAction

An automatically ending action that you want to perform on a vehicle.

struct FunctionIdentifier

A type that stores the designation code for one of your vehicle’s features.

struct ActionIdentifier

A type that stores the designation code for one of the actions that a vehicle feature supports.

