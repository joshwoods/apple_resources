

- CarKey
- CarKeyRemoteControlSession
-  sendPassthroughData(\_:toVehicle:) 

Instance Method

# sendPassthroughData(\_:toVehicle:)

Sends the specified custom data to the vehicle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func sendPassthroughData(
    _ passthroughData: Data,
    toVehicle vehicleID: String
) throws
```

## Parameters 

`passthroughData`  

The custom data to send to the vehicle. Make sure the size of your data object doesn’t exceed 65 kilobytes.

`vehicleID`  

The target vehicle for the request. Choose the vehicle from one of the session’s vehicle reports. Specify the string in the identifier property of the corresponding report.

## Discussion

Use this method to send data that is custom to your specific vehicle. This method passes the data unmodified directly to the vehicle, and it is up to you to format the data exactly how the vehicle needs it.

If the vehicle sends a custom response, the system delivers it to the remoteControlSession(_:didReceivePassthroughData:fromVehicle:) method of your session’s delegate object.

