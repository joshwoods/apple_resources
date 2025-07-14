

- Core Media I/O
- CMIOExtensionProperty
-  streamFrameDuration 

Type Property

# streamFrameDuration

A property key for the frame duration.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let streamFrameDuration: CMIOExtensionProperty
```

## Discussion

The property state for this property is a dictionary that represents a doc://com.apple.documentation/documentation/coremedia/cmtime-u58 value that matches the frame duration of the active stream format.

## See Also

### Stream Properties

static let streamActiveFormatIndex: CMIOExtensionProperty

A property key for the index of the active stream format.

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

