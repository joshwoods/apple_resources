

- Core Media I/O
- CMIOExtensionProperty
-  streamSinkEndOfData 

Type Property

# streamSinkEndOfData

A property key for a Boolean value that indicates whether the stream has more data.

Mac Catalyst 15.4+macOS 12.3+

``` source
static let streamSinkEndOfData: CMIOExtensionProperty
```

## Discussion

The property state for this property is a number that represents a Boolean value: `1` indicates the stream is at its end, and `0` indicates that more data exists.

The value of this property matches the kCMIOStreamPropertyEndOfData property.

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

static let streamSinkBufferUnderrunCount: CMIOExtensionProperty

A property key for the buffer underrun count.

