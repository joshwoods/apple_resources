

- CarKey
- CarKeyRemoteControlSession
-  isPassiveEntryAvailable(forVehicle:) 

Instance Method

# isPassiveEntryAvailable(forVehicle:)

Returns a Boolean value that indicates whether passive entry is currently available for the specified vehicle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func isPassiveEntryAvailable(forVehicle vehicleID: String) throws -> Bool
```

## Parameters 

`vehicleID`  

The target vehicle for the request. Choose the vehicle from one of the session’s vehicle reports. Specify the string in the identifier property of the corresponding report.

## Return Value

`true` if passive entry is available, or `false` if the feature is not available.

## See Also

### Getting Vehicle Information

var vehicleReports: [VehicleReport]

The configuration details of the provisioned vehicles that match your company’s make.

