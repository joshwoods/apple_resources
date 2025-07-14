

- Core Media I/O
- CMIOExtensionStream
-  clockType 

Instance Property

# clockType

A clock type for the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
var clockType: CMIOExtensionStream.ClockType { get }
```

## Discussion

If you created the stream with a custom clock configuration, the value of this property is CMIOExtensionStream.ClockType.custom.

## See Also

### Inspecting a Stream

var source: (any CMIOExtensionStreamSource)?

The source object for the stream.

var direction: CMIOExtensionStream.Direction

The data-flow direction of the stream.

enum Direction

Constants that define the data-flow direction of the stream.

enum ClockType

Constants that indicate the clock type of a stream.

var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration?

An optional custom clock configuration for a stream.

class CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

