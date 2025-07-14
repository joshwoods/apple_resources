

- Core Media I/O
- CMIOExtensionStream
-  customClockConfiguration 

Instance Property

# customClockConfiguration

An optional custom clock configuration for a stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration? { get }
```

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

enum ClockType

Constants that indicate the clock type of a stream.

class CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

