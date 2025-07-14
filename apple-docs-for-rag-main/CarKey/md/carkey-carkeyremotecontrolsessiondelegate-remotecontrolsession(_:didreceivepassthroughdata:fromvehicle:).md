

- CarKey
- CarKeyRemoteControlSessionDelegate
-  remoteControlSession(\_:didReceivePassthroughData:fromVehicle:) 

Instance Method

# remoteControlSession(\_:didReceivePassthroughData:fromVehicle:)

Notifies the delegate object that the vehicle sent passthrough data for you to handle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func remoteControlSession(
    _ session: CarKeyRemoteControlSession,
    didReceivePassthroughData: Data,
    fromVehicle vehicleID: String
)
```

**Required**

## Parameters 

`session`  

The current session.

`didReceivePassthroughData`  

The passthrough data that the vehicle sent. Use the data to determine what actions to take, if any.

`vehicleID`  

The identifier of the vehicle that sent the data. This identifier is the same string in the identifier property of the vehicle report.

## Discussion

If the vehicle sends data, the system delivers it to your app using this method. You are responsible for the data your vehicles produce, and for decoding that data in your implementation of this method. The session doesn’t save or modify the data in any way.

The system executes this method on the dispatch queue you specified when you started the session.

## See Also

### Receiving Data from the Vehicle

func remoteControlSession(CarKeyRemoteControlSession, vehicleDidUpdateReport: VehicleReport)

Notifies your delegate object that the status of the specified vehicle changed.

**Required**

