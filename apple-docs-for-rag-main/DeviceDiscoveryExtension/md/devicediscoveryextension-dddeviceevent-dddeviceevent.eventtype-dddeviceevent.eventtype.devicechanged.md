

- DeviceDiscoveryExtension
- DDDeviceEvent
- DDDeviceEvent.EventType
-  DDDeviceEvent.EventType.deviceChanged 

Case

# DDDeviceEvent.EventType.deviceChanged

A status that indicates when the device of interest changes configuration.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
case deviceChanged
```

## Discussion

Report an event of this type to notify the system when information about a discovered device changes, for example, when:

- Adding or losing a communication protocol.

- Updating information about the current media that the device plays.

## See Also

### Distinguishing event types

case unknown

A value for uninitialized event types.

case deviceFound

A status that indicates when the extension finds the device of interest.

case deviceLost

A status that indicates when the extension loses a connection to the device of interest.

