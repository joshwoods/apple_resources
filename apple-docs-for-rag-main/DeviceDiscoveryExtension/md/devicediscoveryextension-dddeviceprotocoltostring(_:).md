

- DeviceDiscoveryExtension
-  DDDeviceProtocolToString(\_:) 

Function

# DDDeviceProtocolToString(\_:)

Returns human-readable text for the specified protocol identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
func DDDeviceProtocolToString(_ inValue: DDDevice.Protocol) -> String
```

## Parameters 

`inValue`  

A device-protocol identifier to convert to text.

## Return Value

A textual value for the specified device protocol.

## Discussion

Your extension can use this function for logging.

## See Also

### Device information

class DDDevice

An object that describes a discovered device of interest.

enum Category

An option that determines the icon for the device in the picker UI.

enum DDDeviceState

A state that represents the level of user interaction with the device.

func DDDeviceCategoryToString(DDDevice.Category) -> String

Returns human-readable text for the specified identifier that describes a device’s category.

func DDDeviceStateToString(DDDeviceState) -> String

Returns human-readable text for the specified identifier that describes a device’s status.

enum Protocol

An identifier for the manner in which an app interacts with a device.

struct DDDeviceProtocolString

String values for the manner in which an app interacts with a device.

func DDDeviceMediaPlaybackStateToString(DDDevice.MediaPlaybackState) -> String

Returns human-readable text for the specified media playback state.

