

- Core Media I/O
- CMIOExtensionProperty
-  deviceIsSuspended 

Type Property

# deviceIsSuspended

A property key for a Boolean value that indicates whether the device is in a suspended state.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let deviceIsSuspended: CMIOExtensionProperty
```

## Discussion

An example of when a device may be in a suspended state is when a user closes their laptop. While suspended, the device continues to respond to requests as if it were active, but the stream doesn’t provide any data.

The property state for this property is a number that represents a Boolean value.

## See Also

### Device Properties

static let deviceModel: CMIOExtensionProperty

A property key for the device model.

static let deviceTransportType: CMIOExtensionProperty

A property key for the device transport type.

static let deviceLinkedCoreAudioDeviceUID: CMIOExtensionProperty

A property key for the UID of the linked Core Audio device.

static let deviceCanBeDefaultInputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default input device.

static let deviceCanBeDefaultOutputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default output device.

