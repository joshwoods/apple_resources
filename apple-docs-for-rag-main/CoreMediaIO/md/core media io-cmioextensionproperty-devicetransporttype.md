

- Core Media I/O
- CMIOExtensionProperty
-  deviceTransportType 

Type Property

# deviceTransportType

A property key for the device transport type.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let deviceTransportType: CMIOExtensionProperty
```

## Discussion

The property state for this property is a number value that corresponds to an audio transport type (`kIOAudioDeviceTransportType`) that the IOKit framework defines.

## See Also

### Device Properties

static let deviceModel: CMIOExtensionProperty

A property key for the device model.

static let deviceIsSuspended: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device is in a suspended state.

static let deviceLinkedCoreAudioDeviceUID: CMIOExtensionProperty

A property key for the UID of the linked Core Audio device.

static let deviceCanBeDefaultInputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default input device.

static let deviceCanBeDefaultOutputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default output device.

