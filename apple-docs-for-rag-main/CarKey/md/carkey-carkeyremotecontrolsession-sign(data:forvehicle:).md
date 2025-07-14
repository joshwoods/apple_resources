

- CarKey
- CarKeyRemoteControlSession
-  sign(data:forVehicle:) 

Instance Method

# sign(data:forVehicle:)

Sign data with the endpoint.SK identified by vehicleIdentifier as described in the section “OEM App Data Attestation” of the Car Connectivity Consortium Digital Key Release 3.0 specification.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func sign(
    data: Data,
    forVehicle vehicleID: String
) throws -> CarKeyRemoteControlSession.Attestation
```

## Parameters 

`data`  

The OEM App Data to sign.

`vehicleID`  

The vehicle identifier.

## Return Value

An Attestation object.

## Discussion

This method can only be used while the application is in the foreground.

