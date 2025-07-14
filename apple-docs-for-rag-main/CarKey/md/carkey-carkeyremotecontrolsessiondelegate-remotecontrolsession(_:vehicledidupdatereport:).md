

- CarKey
- CarKeyRemoteControlSessionDelegate
-  remoteControlSession(\_:vehicleDidUpdateReport:) 

Instance Method

# remoteControlSession(\_:vehicleDidUpdateReport:)

Notifies your delegate object that the status of the specified vehicle changed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func remoteControlSession(
    _ session: CarKeyRemoteControlSession,
    vehicleDidUpdateReport: VehicleReport
)
```

**Required**

## Parameters 

`session`  

The current session.

`vehicleDidUpdateReport`  

The updated vehicle report, which you can use to make changes immediately.

## Discussion

When information for a vehicle changes, the session notifies its delegate so you can make any changes. To save time, use the provided report rather than requesting the report again from the session’s vehicleReports property. The system executes this method on the dispatch queue you specified when you started the session.

## See Also

### Receiving Data from the Vehicle

func remoteControlSession(CarKeyRemoteControlSession, didReceivePassthroughData: Data, fromVehicle: String)

Notifies the delegate object that the vehicle sent passthrough data for you to handle.

**Required**

