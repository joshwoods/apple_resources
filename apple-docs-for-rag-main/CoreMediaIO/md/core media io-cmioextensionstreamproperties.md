

- Core Media I/O
-  CMIOExtensionStreamProperties 

Class

# CMIOExtensionStreamProperties

An object that describes the properties of an extension stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionStreamProperties
```

## Topics

### Creating Stream Properties

init(dictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Creates a properties object that provides the specified properties and default states.

### Configuring Sink Properties

var sinkBufferQueueSize: Int?

The buffer queue size.

var sinkBuffersRequiredForStartup: Int?

The number of buffers the stream requires for startup.

var sinkBufferUnderrunCount: Int?

The buffer underrun count.

var sinkEndOfData: Int?

A value that indicates whether the stream has reached its end.

### Configuring Source Properties

var activeFormatIndex: Int?

The index of the active format.

var frameDuration: CMTime?

The duration of the frame.

var maxFrameDuration: CMTime?

The maximum duration of a frame.

### Managing Property State

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary representation of the property state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the state of the specified property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Streams

class CMIOExtensionStream

An object that represents a stream of media data.

protocol CMIOExtensionStreamSource

A protocol for objects that act as stream sources.

class CMIOExtensionClient

An object that represents a client of the extension.

