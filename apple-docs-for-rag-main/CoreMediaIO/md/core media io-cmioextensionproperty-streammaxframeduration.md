

- Core Media I/O
- CMIOExtensionProperty
-  streamMaxFrameDuration 

Type Property

# streamMaxFrameDuration

A property key for the maximum frame duration.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let streamMaxFrameDuration: CMIOExtensionProperty
```

## Discussion

The property state for this property is a dictionary representation of a doc://com.apple.documentation/documentation/coremedia/cmtime-u58 structure.

## See Also

### Stream Properties

static let streamActiveFormatIndex: CMIOExtensionProperty

A property key for the index of the active stream format.

static let streamFrameDuration: CMIOExtensionProperty

A property key for the frame duration.

static let streamSinkBufferQueueSize: CMIOExtensionProperty

A property key for the sink buffer queue size.

static let streamSinkBuffersRequiredForStartup: CMIOExtensionProperty

A property key for the number of buffers required for startup.

static let streamSinkBufferUnderrunCount: CMIOExtensionProperty

A property key for the buffer underrun count.

static let streamSinkEndOfData: CMIOExtensionProperty

A property key for a Boolean value that indicates whether the stream has more data.

