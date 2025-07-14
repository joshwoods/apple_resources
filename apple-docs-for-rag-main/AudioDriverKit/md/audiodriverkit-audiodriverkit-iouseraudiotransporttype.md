

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioTransportType 

Enumeration

# IOUserAudioTransportType

The type of transport to deliver audio.

DriverKit 21.0+

``` source
enum IOUserAudioTransportType : uint32_t;
```

## Topics

### Protocol-based Transport Types

PCI

The transport type ID for audio devices connected with the PCI bus.

USB

The transport type ID for audio devices connected with USB.

FireWire

The transport type ID for audio devices connected with FireWire.

Bluetooth

The transport type ID for audio devices connected with Bluetooth.

BluetoothLE

The transport type ID for audio devices connected with Bluetooth Low Energy.

HDMI

The transport type ID for audio devices connected with HDMI.

DisplayPort

The transport type ID for audio devices connected with DisplayPort.

AirPlay

The transport type ID for audio devices connected with AirPlay.

AVB

The transport type ID for audio devices connected with Audio Video Bridging (AVB).

Thunderbolt

The transport type ID for audio devices connected with Thunderbolt.

### Other Transport Types

Unknown

The transport type ID returned when a device doesn’t provide a transport type.

BuiltIn

The transport type ID for AudioDevices built into the system.

## See Also

### Working with Transport Types

SetTransportType

Sets the box’s transport type.

GetTransportType

Returns the box’s transport type.

