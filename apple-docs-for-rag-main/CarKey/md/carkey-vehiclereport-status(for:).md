

- CarKey
- VehicleReport
-  status(for:) 

Instance Method

# status(for:)

Returns the current status of the specified vehicle function.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func status(for function: FunctionIdentifier) throws -> FunctionStatus?
```

## Parameters 

`function`  

The function identifier for the vehicle feature you want to check. If you specify an unknown feature, this method throws an error. For a list of the vehicle’s supported features, see the supportedFunctions property.

## Return Value

The status of the feature, or `nil` if the status is currently unknown.

## Discussion

Each feature of your vehicle has one or more associated states, which you define. For example, the door locks of a vehicle might be in the locked or unlocked state. This method returns the state if it is known.

## See Also

### Getting the Vehicle’s Supported Functions

var supportedFunctions: [FunctionIdentifier]

An array of function identifiers that indicates the features the vehicle supports, populated only after the first BLE connection with the vehicle.

struct FunctionStatus

A value that the vehicle can return to indicate the status of a particular vehicle feature.

