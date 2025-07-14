

- Core Media I/O
- CMIOExtensionStream
-  CMIOExtensionStream.ClockType 

Enumeration

# CMIOExtensionStream.ClockType

Constants that indicate the clock type of a stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
enum ClockType
```

## Topics

### Clock Types

case hostTime

Indicates that the stream uses the host time clock.

case linkedCoreAudioDeviceUID

Indicates that the stream uses the clock of the linked Core Audio device.

case custom

Indicates that the stream’s clock is specific to the device hosting the stream.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Stream

var source: (any CMIOExtensionStreamSource)?

The source object for the stream.

var direction: CMIOExtensionStream.Direction

The data-flow direction of the stream.

enum Direction

Constants that define the data-flow direction of the stream.

var clockType: CMIOExtensionStream.ClockType

A clock type for the stream.

var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration?

An optional custom clock configuration for a stream.

class CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

