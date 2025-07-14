

- Core Media I/O
- CMIOExtensionProperty
-  deviceLinkedCoreAudioDeviceUID 

Type Property

# deviceLinkedCoreAudioDeviceUID

A property key for the UID of the linked Core Audio device.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let deviceLinkedCoreAudioDeviceUID: CMIOExtensionProperty
```

## Discussion

The property state for this property is a string with a read-only attribute.

## See Also

### Device Properties

static let deviceModel: CMIOExtensionProperty

A property key for the device model.

static let deviceIsSuspended: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device is in a suspended state.

static let deviceTransportType: CMIOExtensionProperty

A property key for the device transport type.

static let deviceCanBeDefaultInputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default input device.

static let deviceCanBeDefaultOutputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default output device.

