

- DeviceDiscoveryExtension
- DDDevice
-  supportsGrouping 

Instance Property

# supportsGrouping

A Boolean value that indicates whether to group the device with others in the AirPlay UI.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+

``` source
var supportsGrouping: Bool { get set }
```

## Discussion

This property provides a convenient way to send the same media stream to multiple devices and list them as a group in the AirPlay UI (AVRoutePickerView). For example, a set of speakers arranged around the room can implement stereo playback by each playing different audio channels from an audio stream.

When someone selects a media receiver in the AirPlay menu, the system checks if it supports grouping. If so, the AirPlay UI displays a checkbox next to any other media receivers that also support grouping and implement the same protocol (DDDevice.Protocol).

If a person selects multiple devices in the menu, the selected devices reorder next to each other in the list.

Note

Implement didReceiveEvent(_:) in the DDDiscoveryExtension to detect when a person changes the device grouping using the AirPlay UI.

## See Also

### Setting the device state

var state: DDDeviceState

A state that represents the level of user interaction with the device.

var txtRecord: NWTXTRecord?

A dictionary of metadata for the device that the extension communicates with over the local network.

var url: URL

A resource locator for the simple service discovery protocol.

