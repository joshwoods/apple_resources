

- Core Media I/O
- CMIOExtensionProperty
-  streamSinkBufferUnderrunCount 

Type Property

# streamSinkBufferUnderrunCount

A property key for the buffer underrun count.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let streamSinkBufferUnderrunCount: CMIOExtensionProperty
```

## Discussion

The system updates this value every time you don’t service a stream’s buffer fast enough.

The property state for property is a number with a read-only attribute. The value of this property matches the value of the kCMIOStreamPropertyOutputBufferUnderrunCount property.

## See Also

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

static let streamSinkEndOfData: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the stream has more data.

