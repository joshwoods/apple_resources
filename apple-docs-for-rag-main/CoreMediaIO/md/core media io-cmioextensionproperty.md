

- Core Media I/O
-  CMIOExtensionProperty 

Structure

# CMIOExtensionProperty

A structure that defines the properties that providers, devices, and streams support.

Mac Catalyst 15.4+macOS 12.3+

``` source
struct CMIOExtensionProperty
```

## Topics

### Provider Properties

static let providerName: CMIOExtensionProperty

A property key for the provider name.

static let providerManufacturer: CMIOExtensionProperty

A property key for the provider manufacturer.

### Device Properties

static let deviceModel: CMIOExtensionProperty

A property key for the device model.

static let deviceIsSuspended: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device is in a suspended state.

static let deviceTransportType: CMIOExtensionProperty

A property key for the device transport type.

static let deviceLinkedCoreAudioDeviceUID: CMIOExtensionProperty

A property key for the UID of the linked Core Audio device.

static let deviceCanBeDefaultInputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default input device.

static let deviceCanBeDefaultOutputDevice: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the device can be a default output device.

### Stream Properties

static let streamActiveFormatIndex: CMIOExtensionProperty

A property key for the index of the active stream format.

static let streamFrameDuration: CMIOExtensionProperty

A property key for the frame duration.

static let streamMaxFrameDuration: CMIOExtensionProperty

A property key for the maximum frame duration.

static let streamSinkBufferQueueSize: CMIOExtensionProperty

A property key for the sink buffer queue size.

static let streamSinkBuffersRequiredForStartup: CMIOExtensionProperty

A property key for the number of buffers required for startup.

static let streamSinkBufferUnderrunCount: CMIOExtensionProperty

A property key for the buffer underrun count.

static let streamSinkEndOfData: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the stream has more data.

### Type Properties

static let deviceLatency: CMIOExtensionProperty

static let streamLatency: CMIOExtensionProperty

init(rawValue: String)

Creates a property with a raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Properties

class CMIOExtensionPropertyState

An object that describes the state of a property.

class CMIOExtensionPropertyAttributes

An object that describes the attributes of a property.

let CMIOExtensionInfoDictionaryKey: String

A key that specifies the extension information dictionary.

let CMIOExtensionMachServiceNameKey: String

A key that specifies the mach service name.

