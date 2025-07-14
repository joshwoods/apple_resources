

- Core Media I/O
- CMIOExtensionProperty
-  streamSinkBufferQueueSize 

Type Property

# streamSinkBufferQueueSize

A property key for the sink buffer queue size.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let streamSinkBufferQueueSize: CMIOExtensionProperty
```

## Discussion

The property state for this property is a number. The property value matches the value of the kCMIOStreamPropertyOutputBufferQueueSize property.

## See Also

### Stream Properties

static let streamActiveFormatIndex: CMIOExtensionProperty

A property key for the index of the active stream format.

static let streamFrameDuration: CMIOExtensionProperty

A property key for the frame duration.

static let streamMaxFrameDuration: CMIOExtensionProperty

A property key for the maximum frame duration.

static let streamSinkBuffersRequiredForStartup: CMIOExtensionProperty

A property key for the number of buffers required for startup.

static let streamSinkBufferUnderrunCount: CMIOExtensionProperty

A property key for the buffer underrun count.

static let streamSinkEndOfData: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the stream has more data.

